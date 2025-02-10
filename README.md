# LiteRT for Dart web

Fork of: 

Run TFLite models on Dart JS. It is packaged in a WebAssembly binary that runs in a browser

## Getting Started

Get the binaries:

```
TODO
```

+ Initialize:
```
await TFLiteWeb.initialize();
```
This may take a couple of seconds
+ Either Load Model from Url:
```
final loadedModel = await TFLiteModel.fromUrl(modelUrl);
```
+ Or load from memory:
```
final loadedModel = await TFLiteModel.fromMemory(modelBytes);
```
+ Create a tensor:
```
final input = createTensor(data, shape, dataType);
```
+ Run the model:
```
final outputs = loadedModel.predict(input);
```
Depending on the model, the input can be a Tensor, a list of Tensors, or a Tensor map


## Current Version:
+ TF-JS: 4.11.0
+ TF-JS TFLite: 0.0.1-alpha.10
