# example W3C Web annotation from Golden Agents

In this annotation the `tagging` and `commenting` `body`s combined with the `TextPositionSelector` and `TextQuoteSelector` in the `target` are compatible with the use of recogito-js for displaying the annotations in the text.

```
{
    "@context": [
        "http://www.w3.org/ns/anno.jsonld",
        {
            "match_phrase": "urn:golden-agents:match_phrase",
            "match_variant": "urngolden-agents:match_variant",
            "match_score": "urn:golden-agents:match_score",
            "category": "urn:example:golden-agents:category"
        }
    ],
    "id": "1ecd0e5e-bc57-4a66-96cd-e0899b055505",
    "type": "Annotation",
    "motivation": "classifying",
    "generated": "2022-02-16T15:32:01.650990",
    "generator": {
        "id": "https://github.com/knaw-huc/golden-agents-htr",
        "type": "Software",
        "name": "GoldenAgentsNER"
    },
    "body": [
        {
            "type": "TextualBody",
            "value": "firstname",
            "modified": "2022-02-16T15:32:01.650949",
            "purpose": "tagging"
        },
        {
            "type": "TextualBody",
            "value": "familyname",
            "modified": "2022-02-16T15:32:01.650962",
            "purpose": "tagging"
        },
        {
            "type": "TextualBody",
            "value": "Carel",
            "modified": "2022-02-16T15:32:01.650965",
            "purpose": "commenting"
        },
        {
            "type": "TextualBody",
            "value": [
                "firstname",
                "familyname"
            ],
            "purpose": "classifying"
        },
        {
            "type": "Dataset",
            "value": {
                "match_phrase": "arel",
                "match_variant": "Carel",
                "match_score": 0.5983173076923077,
                "category": [
                    "firstname",
                    "familyname"
                ]
            }
        }
    ],
    "target": {
        "source": "urn:golden-agents:unknown:scan=A16097000219",
        "selector": [
            {
                "type": "TextPositionSelector",
                "start": 8,
                "end": 12
            },
            {
                "type": "TextQuoteSelector",
                "exact": "arel"
            }
        ]
    }
}
```
