# Shape

## 対応できそうか？

### できそう？

- Rectangle
- Oval
- Star
- Polygon

### そのまま(できない)

- Line
- Curve
- Spiral

Neither は無視でも PowerStroke の時に使うことになる？？

## Curve 44

paths にある値

### rectangle

shapeDescription になる

```json
"inputParams": {
    "shapeDescription": {
        "_0": "(rectangle)"
    }
}
```

**参考**

### Curve 40

elementDescription があるのに...

つまり shape があるかどうかで分岐をすべきか?
それとも初めから全部 Path 由来で作る方がいいのか?
(それだと shape.py いらなくなる, shapeDescription がカギになる)

```json
"inputParams": {
    "neither": {}
}
```

### Curve 21

Vectornator に最も近い(primitive)

```json
"inputParams": {
    "shape": {
        "_0": {
            "endPoint": [
                446.71444440772575,
                218.13256133889018
            ],
            "additionalValue": {
                "rectangle": {
                    "cornerRadius": 4
                }
            },
            "initialPoint": [
                21.992140203976316,
                165.91616952857868
            ]
        }
    }
}
```

---

### oval

```json
"inputParams": {
    "shapeDescription": {
        "_0": "(oval)"
    }
}
```

---

### star

(star)がなぜかない (つまり shapeDescription を取得できない)
これは(star), (polygon), (spiral) で共通

```json
"inputParams": {
    "shape": {
        "_0": {
            "additionalValue": {
                "star": {
                    "innerRadius": 1.003989732950315,
                    "numberOfPoints": 5
                }
            },
            "endPoint": [
                0,
                -162.7726601884978
            ],
            "initialPoint": [
                5.684341886080802e-14,
                17.18436696451579
            ]
        }
    }
}
```

---

### polygon

```json
"inputParams": {
    "shape": {
        "_0": {
            "additionalValue": {
                "polygon": {
                    "numberOfSides": 5
                }
            },
            "endPoint": [
                -8.526512829121202e-14,
                102.05051078085432
            ],
            "initialPoint": [
                -5.684341886080802e-14,
                -10.773759083028267
            ]
        }
    }
}
```

---

### spiral

```json
"inputParams": {
    "shape": {
        "_0": {
            "additionalValue": {
                "spiral": {
                    "decay": 88
                }
            },
            "endPoint": [
                -76.51959076922935,
                -185.75334978733494
            ],
            "initialPoint": [
                49.17405936352134,
                -6.89097289121429
            ]
        }
    }
}
```

---

### line

```json
"inputParams": {
    "shapeDescription": {
        "_0": "(line)"
    }
}
```

---

### curve

```json
"inputParams": {
    "shapeDescription": {
        "_0": "(curve)"
    }
}
```

## Vectornator 14

element 直下に"elementDescription"が存在する

pathData.\_0.subElement 以下にある

### "(rectangle)"

```json
"subElement": {
    "shape": {
        "_0": {
            "endPoint": [
                188.85442578376305,
                112.57381741261761
            ],
            "additionalValue": {
                "rectangle": {
                    "cornerRadius": 0
                }
            },
            "initialPoint": [
                9.53989031760753,
                52.473202007023986
            ]
        }
    }
}
```

---

### "(oval)"

oval はどのバージョンでも一から作り直すしかない

transform をなくしてから width, height を測るだけだと思う
これは inkex.Path からでいいはず

```json
"subElement": {
    "neither": {}
}
```

---

### "(star)"

```json
"subElement": {
    "shape": {
        "_0": {
            "endPoint": [
                99.94007668467819,
                194.68821229054998
            ],
            "additionalValue": {
                "star": {
                    "numberOfPoints": 5,
                    "innerRadius": 0.5
                }
            },
            "initialPoint": [
                85.1964149572947,
                283.08809409677923
            ]
        }
    }
}
```

---

### "(polygon)"

```json
"subElement": {
    "shape": {
        "_0": {
            "endPoint": [
                315.3451942921021,
                446.30483712595327
            ],
            "initialPoint": [
                342.00735209202924,
                516.7363901733286
            ],
            "additionalValue": {
                "polygon": {
                    "numberOfSides": 5
                }
            }
        }
    }
}
```

---

### "(spiral)"

```json
"subElement": {
    "shape": {
        "_0": {
            "endPoint": [
                449.0994768344138,
                187.69661997781995
            ],
            "additionalValue": {
                "spiral": {
                    "decay": 88
                }
            },
            "initialPoint": [
                378.2014552421003,
                101.2738090058707
            ]
        }
    }
}
```

---

### "(line)"

```json
"subElement": {
    "neither": {}
}
```

---

### "(curve)"

```json
"subElement": {
    "neither": {}
}
```
