## Hi there 👋
### Welcome to WebARKit !!

<div align="center">

# 🖼️ WebARKit

**A new place for the development of the WebAR of tomorrow.**

Open-source WebAR tooling — from historical tracking in C/C++ to pure-Rust, WASM-first computer vision.

[![Website](https://img.shields.io/badge/website-webarkit.org-blue)](https://webarkit.org)
[![Twitter](https://img.shields.io/badge/twitter-@webarkit-1DA1F2?logo=twitter&logoColor=white)](https://twitter.com/webarkit)
contact@webarkit.org

</div>

---

## 🙋 Who we are

We are a group of developers passionate about **Web Augmented Reality**. We believe open source makes a difference: we build libraries for marker-based and markerless (NFT) tracking directly in the browser, without plugins, using WebAssembly.

Our work covers the entire stack: from historical bindings based on ARToolKit to a new generation of **pure-Rust** libraries, designed to be lightweight, portable (including `no_std`), and performant on WASM.

---

## 🚀 Main Projects

### New Generation (Rust / WASM)

| Project | Description |
|---|---|
| [**PureCV**](https://github.com/webarkit/PureCV) | Computer vision library in pure Rust, without FFI dependencies, designed for the WASM target. On the roadmap: Feature detection (TEBLID, FREAK, StarDetector/CenSurE) and matching (BFMatcher, GMS filtering), with experimental `no_std` support under evaluation. |
| [**WebARKitLib-rs**](https://github.com/webarkit/WebARKitLib-rs) | Rewrite of the WebAR tracking library in Rust, a direct successor to WebARKitLib/ARToolKit5, designed to compile efficiently to WASM. |
| [**jsfeatNext**](https://github.com/webarkit/jsfeatNext) | TypeScript version of jsfeat, with type definitions, used as a computer vision layer on the JS/TS side. |
| [**webarkit**](https://github.com/webarkit/webarkit) | 🚧 *Proposed.* Organization's central repo: will host the shared CV contract (@webarkit/cv-backend-spec), making jsfeatNext and PureCV backends interchangeable for a future high-level AR project. |

### Historical Library (C/C++)

| Project | Description |
|---|---|
| [**WebARKitLib**](https://github.com/webarkit/WebARKitLib) | The C/C++ source code for WebARKit, based on ARToolKit5 and extended with new features (SIMD, logging, improved tracking). |
| [**webarkit-cv**](https://github.com/webarkit/webarkit-cv) | WebARKit compiled via Emscripten/OpenCV: the bridge between the C++ library and the browser. |

### Markerless / NFT tracking

| Project | Description |
|---|---|
| [**ARnft**](https://github.com/webarkit/ARnft) | Lightweight JavaScript library for WebAR with markerless tracking (NFT), based on jsartoolkitNFT, with rendering via three.js. |
| [**jsartoolkitNFT**](https://github.com/webarkit/jsartoolkitNFT) | A stripped-down version of jsartoolkit5, focused exclusively on NFT (Natural Feature Tracking) support. |

---

## 🧭 Where we're going

The current focus is migrating to a pure-Rust, FFI-free stack, with particular attention to:

- 📦 WASM binary size control
- 🔧 `no_std` compatibility (embedded target, e.g., ESP32)
- ⚡ SIMD performance on WASM
- 🧩 API consistency across different repositories

On the C/C++ side, work hasn't stopped: recent tracking improvements (first-frame robustness, marker-centered origin option) and the OpenCV/Emscripten pipeline update are keeping the historical foundation solid as the Rust stack matures.

🚧 **In discussion:** A proposal for a monorepo hosting a **shared CV contract** (`@webarkit/cv-backend-spec`) is open in the [`webarkit`](https://github.com/webarkit/webarkit) repo, making jsfeatNext and PureCV interchangeable backends behind the same interface, ready to be consumed by a future high-level AR project. The status is still *draft*, open to discussion about the monorepo structure and package names.

## 🤝 Contribute

Pull requests are welcome! Check out the open issues in the individual repositories—many are labeled `good first issue` or `help wanted`. For general questions, you can email us at contact@webarkit.org or visit [webarkit.org](https://webarkit.org).
