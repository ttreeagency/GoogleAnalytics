[![BSD License](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)
[![Latest Stable Version](https://poser.pugx.org/ttree/googleanalytics/version)](https://packagist.org/packages/ttree/googleanalytics)

# Google Analytics TS Object

This package contains a TypoScript object to integrate Google Analytics tracking code in your Neos CMS project.

## How to integrate your tracking code?

Add this to your TypoScript to add the tracking snippet and set your code:

    prototype(TYPO3.Neos:Page)
        body.javascripts.analytics = Ttree.GoogleAnalytics:TrackingCode {
            trackingCode = 'UA-...'
        }
    }

**Note:** By default the tracking code is included only in ```Production``` context. If you need to include the tracking code
also in ```Development``` context, check the code in [TrackingCode](Resources/Private/TypoScript/TypoScriptObjects/TrackingCode.ts2),
you can adjust the Eel expression at ```@if.includeTrackingCode``` as you need.

## Acknowledgments

Development sponsored by [ttree ltd - neos solution provider](http://ttree.ch).

We try our best to craft this package with a lots of love, we are open to sponsoring, support request, ... just contact us.

## License

The MIT License (MIT). Please see [LICENSE](LICENSE) for more information.
