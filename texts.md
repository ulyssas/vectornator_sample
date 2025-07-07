# Texts

## Curve 44

### normal
```json
"fillColor": {
    "values": [
        {
            "upperBound": 7,
            "value": {
                "hsba": {
                    "alpha": 1,
                    "brightness": 1,
                    "hue": 0,
                    "saturation": 1
                }
            }
        }
    ]
}
```


### stroke
textにあるstrokeStyleは二つ(color, width)に分かれている

Vectornatorでもそうだが各文字に固有なのはcolor, widthのみ

basicStrokeStyle(全て共通)に相当する部分はtextStrokeStylesにある

```json
"strokeStyle": {
    "color": {
        "values": [
            {
                "upperBound": 6,
                "value": {
                    "hsba": {
                        "alpha": 1,
                        "brightness": 0,
                        "hue": 0,
                        "saturation": 0
                    }
                }
            }
        ]
    },
    "width": {
        "values": [
            {
                "upperBound": 6,
                "value": 3
            }
        ]
    }
}

"textStrokeStyles": [
    {
        "cap": 0,
        "dashPattern": [
            1,
            0,
            0,
            0
        ],
        "join": 0,
        "position": 0
    }
]
```

これをこうしたい

```json
{
    "basicStrokeStyle": {
        "cap": 0,
        "dashPattern": [
            0,
            0,
            0,
            0
        ],
        "join": 1,
        "position": 0
    },
    "color": {
        "hsba": {
            "alpha": 1,
            "brightness": 0,
            "hue": 0.1755852848291397,
            "saturation": 0
        }
    },
    "endArrow": "open square",
    "startArrow": "arrow1",
    "width": 10
}
```

## Curve 21

VectornatorではattributedTextと同じ階層に位置していた

```json
{
    "width": 576.1843487435294,
    "fontName": "ToppanBunkyuMidashiGothicStdN-ExtraBold",
    "fontSize": 112,
    "resizeMode": 2,
    "height": 126.35371792272815,
    "transform": [
        1,
        0,
        0,
        1,
        223.90782562823563,
        359.62703625853334
    ],
    "alignment": 1
}
```


## Vectornator 14

### stroke
```json
{
    "NSString": "Stroke",
    "NSDelegate": None,
    "NSAttributes": {
        "NSParagraphStyle": {
            "NSTabStops": None,
            "NSTextBlocks": [],
            "NSAllowsTighteningForTruncation": 1,
            "NSTighteningFactorForTruncation": 0.05000000074505806,
            "NSTextLists": [],
            "NSWritingDirection": 1
        },
        "NSStrokeColor": {
            "UIColorComponentCount": 4,
            "UIGreen": 0.0,
            "UIBlue": 0.0,
            "UIAlpha": 1.0,
            "NSRGB": b"0 0 0",
            "UIRed": 0.0,
            "NSColorSpace": 2
        },
        "NSFont": {
            "UIFontMaximumPointSizeAfterScaling": 0.0,
            "UIFontPointSizeForScaling": 0.0,
            "UIFontDescriptor": {
                "UIFontDescriptorOptions": 2147483648,
                "UIFontDescriptorAttributes": {
                    "NSFontSizeAttribute": 40.0,
                    "NSFontNameAttribute": "Helvetica-Bold"
                }
            },
            "NSName": "Helvetica-Bold",
            "NSSize": 40.0,
            "UIFontTraits": 2,
            "UIFontPointSize": 40.0,
            "UIFontTextStyleForScaling": None,
            "UIFontName": "Helvetica-Bold",
            "UISystemFont": False
        },
        "NSStrokeWidth": -3.0
    }
}
```


### styles
```json
{
    "NSString": "Normal Bold Italic Underline Strikethrough  Underline&Strike",
    "NSAttributeInfo": [
        {
            "length": 6,
            "attribute_id": 0
        },
        {
            "length": 6,
            "attribute_id": 1
        },
        {
            "length": 6,
            "attribute_id": 2
        },
        {
            "length": 1,
            "attribute_id": 1
        },
        {
            "length": 9,
            "attribute_id": 3
        },
        {
            "length": 1,
            "attribute_id": 1
        },
        {
            "length": 13,
            "attribute_id": 4
        },
        {
            "length": 2,
            "attribute_id": 0
        },
        {
            "length": 10,
            "attribute_id": 5
        },
        {
            "length": 4,
            "attribute_id": 6
        },
        {
            "length": 2,
            "attribute_id": 5
        }
    ],
    "NSAttributes": [
        {
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            },
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica"
                    }
                },
                "NSName": "Helvetica",
                "NSSize": 18.0,
                "UIFontTraits": 0,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica",
                "UISystemFont": False
            }
        },
        {
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            },
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica-Bold"
                    }
                },
                "NSName": "Helvetica-Bold",
                "NSSize": 18.0,
                "UIFontTraits": 2,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica-Bold",
                "UISystemFont": False
            }
        },
        {
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            },
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica-Oblique"
                    }
                },
                "NSName": "Helvetica-Oblique",
                "NSSize": 18.0,
                "UIFontTraits": 1,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica-Oblique",
                "UISystemFont": False
            }
        },
        {
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica"
                    }
                },
                "NSName": "Helvetica",
                "NSSize": 18.0,
                "UIFontTraits": 0,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica",
                "UISystemFont": False
            },
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSUnderline": 1,
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            }
        },
        {
            "NSStrikethrough": 1,
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica"
                    }
                },
                "NSName": "Helvetica",
                "NSSize": 18.0,
                "UIFontTraits": 0,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica",
                "UISystemFont": False
            },
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            }
        },
        {
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica-BoldOblique"
                    }
                },
                "NSName": "Helvetica-BoldOblique",
                "NSSize": 18.0,
                "UIFontTraits": 3,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica-BoldOblique",
                "UISystemFont": False
            },
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSStrikethrough": 1,
            "NSUnderline": 1,
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            }
        },
        {
            "NSTextEdited": "1",
            "NSStrikethrough": 1,
            "NSUnderline": 1,
            "NSParagraphStyle": {
                "NSTabStops": None,
                "NSTextBlocks": [],
                "NSAllowsTighteningForTruncation": 1,
                "NSTighteningFactorForTruncation": 0.05000000074505806,
                "NSTextLists": [],
                "NSWritingDirection": 1,
                "NSAlignment": 2
            },
            "NSDominantLanguageAttributeName": "en",
            "NSFont": {
                "UIFontMaximumPointSizeAfterScaling": 0.0,
                "UIFontPointSizeForScaling": 0.0,
                "UIFontDescriptor": {
                    "UIFontDescriptorOptions": 2147483648,
                    "UIFontDescriptorAttributes": {
                        "NSFontSizeAttribute": 18.0,
                        "NSFontNameAttribute": "Helvetica-BoldOblique"
                    }
                },
                "NSName": "Helvetica-BoldOblique",
                "NSSize": 18.0,
                "UIFontTraits": 3,
                "UIFontPointSize": 18.0,
                "UIFontTextStyleForScaling": None,
                "UIFontName": "Helvetica-BoldOblique",
                "UISystemFont": False
            },
            "NSColor": {
                "UIColorComponentCount": 4,
                "UIGreen": 0.0,
                "UIBlue": 0.0,
                "UIAlpha": 1.0,
                "NSRGB": b"0 0 0",
                "UIRed": 0.0,
                "NSColorSpace": 2
            },
            "NSDominantScriptAttributeName": "Latn",
            "NSTextChecked": "1"
        }
    ],
    "NSDelegate": None
}
```