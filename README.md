[![BSD License](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)
[![Latest Stable Version](https://poser.pugx.org/ttree/googleanalytics/version)](https://packagist.org/packages/ttree/googleanalytics)

# Google Analytics TS Objects

This package contains TypoScript objects to integrate Google Analytics Tracking code in your Neos CMS project.

## How to integrate your tracking code ?

By default the tracking code in include only in ```Production``` or ```Production/*``` context:

    prototype(TYPO3.Neos:Page)
        body.javascripts.analytics = Ttree.GoogleAnalytics:TrackingCode {
            trackingCode = 'UA-...'
        }
    }

If you need to tracking code check [TrackingCode](Resources/Private/TypoScript/TypoScriptObjects/TrackingCode.ts2), you
can change the EEL expression at ```@if.includeTrackingCode```.

### Additional option

You may enable ```linkid``` feature tracking. [Enhanced Link Attribution](https://support.google.com/analytics/answer/2558867)

    prototype(TYPO3.Neos:Page)
        body.javascripts.analytics = Ttree.GoogleAnalytics:TrackingCode {
            trackingCode = 'UA-...'
            enableLinkId = ${true}
        }
    }


## Acknowledgments

Development sponsored by [ttree ltd - neos solution provider](http://ttree.ch).

We try our best to craft this package with a lots of love, we are open to sponsoring, support request, ... just contact us.

## License

The MIT License (MIT). Please see [LICENSE](LICENSE) for more information.
