## ONNX Runtime CXX on Termux

## WARNING ⚠️

I do not intend to release the code because I don't have it. I did not compile it from scratch; I just used the ONNX binaries compiled for APK (Android) available at https://k2-fsa.github.io/sherpa/onnx/tts/apk.html and replaced them in the original ONNX CXX.

In summary, I used the unzip command on the Next Gen Kaldi TTS, extracted the libonnxruntime.so file from the libs folder, and replaced it in the original code. And it worked.

## OnnxRuntime

ONNX Runtime is a cross-platform machine learning accelerator for inference and training.

Onnxruntime-cxx-termux

To use this on Termux, follow these steps:

1. Update Termux packages:
```
pkg update && pkg upgrade
```

2. Install the necessary C++ dependencies to compile:
```
pkg install clang make
```

3. Install wget and unzip for downloading and extracting files:
```
pkg install wget unzip
```

4. Download the ONNX Runtime package using wget:
```
wget https://github.com/influencia-app/Onnxruntime-cxx-termux/releases/download/release/onnxruntime-linux-aarch64-1.17.0.zip
```

5. Extract the downloaded file using unzip:
```
unzip onnxruntime-linux-aarch64-1.17.0.zip
```

After extracting the files, you can already use it on Termux.

## Thanks 
https://github.com/microsoft/onnxruntime
https://k2-fsa.github.io/sherpa/onnx/tts/apk.html%C2%A0and

License

This project is licensed under the [MIT License](LICENSE).
