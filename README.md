[![BSD License](https://img.shields.io/github/license/mashape/apistatus.svg)](LICENSE)
[![Latest Stable Version](https://poser.pugx.org/ttree/googleanalytics/version)](https://packagist.org/packages/ttree/googleanalytics)

# Google Analytics TS Objects

This package contains TypoScript objects to integrate Google Analytics Tracking code in your Neos CMS project.

## How to integrate your tracking code ?

Generate a HTML script element in HTML5:

    prototype(TYPO3.Neos:Page)
        body.javascripts.analytics = Ttree.GoogleAnalytics:TrackingCode {
            trackingCode = 'UA-...'
        }
    }

## Acknowledgments

Development sponsored by [ttree ltd - neos solution provider](http://ttree.ch).

We try our best to craft this package with a lots of love, we are open to sponsoring, support request, ... just contact us.

## License

The MIT License (MIT). Please see [LICENSE](LICENSE) for more information.
