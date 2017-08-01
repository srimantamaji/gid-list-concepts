## gid-list-concepts

A data component to get list of concepts and its metadata for given user id

    <gid-list-concepts userId='1'></<gid-list-concepts>

API endpoint:

    GET /concepts

Input:

- User Id

Output:

- List of concepts with key metadata (items being displayed on listing page)


The output of this components will be as follows:

    {
      "concepts": [
        {
          "id": "100462",
          "label": "CASE-NUMBER",
          "owner": {
            "id": "111001",
            "label": "Angela"
          },
          "predictedColumns": 0,
          "confirmedColumns": 0,
          "eta": 0,
          "coverage": 0,
          "impactArea": [
            {
              "id": "120002",
              "label": "Credit Risk"
            },
            {
              "id": "120001",
              "label": "GDPR"
            }
          ],
          "classificationAccuracyPercentage": 5,
          "applications": [
            {
              "id": "100492",
              "label": "Universal Biller"
            },
            {
              "id": "100252",
              "label": "Supplier Management Program"
            },
            {
              "id": "100495",
              "label": "Field Service Support"
            },
            {
              "id": "100447",
              "label": "Contract Mgmt System"
            }
          ]
        }    
      ]
    }




## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer serve` to serve your application locally.

## Viewing Your Application

```
$ polymer serve
```

## Building Your Application

```
$ polymer build
```

This will create a `build/` folder with `bundled/` and `unbundled/` sub-folders
containing a bundled (Vulcanized) and unbundled builds, both run through HTML,
CSS, and JS optimizers.

You can serve the built versions by giving `polymer serve` a folder to serve
from:

```
$ polymer serve build/bundled
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
