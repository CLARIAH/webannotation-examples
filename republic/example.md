# Republic example

In this example we annotated several text selections and their corresponding selections on the scan as a `session`, with an appropriate (custom) metdata `DataSet` in the body. The custom fields are defined in its own section of the `@context` since we haven't defined and hosted our custom jsonld context yet.

```
{
        "@context": [
            "http://www.w3.org/ns/anno.jsonld",
            {
                "weekday": "http://example.org/customwebannotationfield#weekday",
                "president": "http://example.org/customwebannotationfield#president",
                "year": "http://example.org/customwebannotationfield#year",
                "date": "http://example.org/customwebannotationfield#date"
            }
        ],
        "id": "urn:example:republic:annotation:df11d729-4866-4d44-b627-2c4157322177",
        "type": "Annotation",
        "motivation": "classifying",
        "generated": "2021-11-18T11:15:58.931772",
        "generator": {
            "id": "https://github.com/knaw-huc/un-t-ann-gle",
            "type": "Software",
            "name": "un-t-ann-gle"
        },
        "body": [
            {
                "type": "TextualBody",
                "purpose": "classifying",
                "value": "session",
                "id": "urn:example:republic:meeting-1728-06-19-session-1"
            },
            {
                "type": "Dataset",
                "value": {
                    "date": "1728-06-19",
                    "year": 1728,
                    "weekday": "Sabbathi",
                    "president": ""
                }
            }
        ],
        "target": [
            {
                "source": "https://demorepo.tt.di.huc.knaw.nl/task/find/volume-1728/file/contents?type=anchor",
                "type": "Text",
                "selector": {
                    "type": "urn:example:republic:TextAnchorSelector",
                    "start": 55952,
                    "end": 56659
                }
            },
            {
                "source": "https://example.org/missing-iiif-url",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/full/,1316/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=1271,2124,891,1116"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/full/,3116/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=2485,439,887,2916"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/full/,304/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=2500,1038,176,104"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/full/,3100/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=3405,435,903,2900"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/full/,3102/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=336,435,881,2902"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/full/,3101/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=1256,432,903,2901"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/full/,3110/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=2480,444,885,2910"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/full/,3106/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=3399,447,895,2906"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/full/,3100/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=344,464,882,2900"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/full/,3100/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=1254,458,908,2900"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/full/,3103/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=2455,474,882,2903"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/full/,3097/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=3368,464,904,2897"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0288.jpg/full/,3056/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=350,455,902,2856"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0288.jpg/full/,1614/0/default.jpg",
                "type": "Image",
                "selector": {
                    "type": "FragmentSelector",
                    "conformsTo": "http://www.w3.org/TR/media-frags/",
                    "value": "xywh=1263,451,907,1414"
                }
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/1271,2124,891,1116/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/2485,439,887,2916/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/2500,1038,176,104/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0285.jpg/3405,435,903,2900/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/336,435,881,2902/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/1256,432,903,2901/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/2480,444,885,2910/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0286.jpg/3399,447,895,2906/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/344,464,882,2900/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/1254,458,908,2900/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/2455,474,882,2903/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0287.jpg/3368,464,904,2897/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0288.jpg/350,455,902,2856/full/0/default.jpg",
                "type": "Image"
            },
            {
                "source": "https://images.diginfra.net/iiif/NL-HaNA_1.01.02/3783/NL-HaNA_1.01.02_3783_0288.jpg/1263,451,907,1414/full/0/default.jpg",
                "type": "Image"
            }
        ]
    }
```