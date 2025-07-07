# Marker

## 問題

パスを途中でトリムできないとマーカーからはみ出てくる

Vectornator ではマーカーも含んだ長さになっている 仕様の違い

あとそれぞれに対応したマーカーも自分で定義する必要がある ここで著作権侵害か？

## Curve 44

pathStrokeStyle に内蔵

```json
{
  "basicStrokeStyle": {
    "cap": 0,
    "dashPattern": [0, 0, 0, 0],
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

## Vectornator 14

strokeStyle に内蔵

```json
"strokeStyle": {
    "position": 0,
    "dashPattern": [
        0,
        0,
        0,
        0
    ],
    "cap": 0,
    "endArrow": "open square",
    "startArrow": "arrow1",
    "color": {
        "s": 0,
        "h": 0.1755852848291397,
        "a": 1,
        "b": 0
    },
    "width": 10,
    "join": 1
}
```
