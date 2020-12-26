<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]



<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/HectorIGH/">
    <img src="README_images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Qonvolution: A Quantum Convolution</h3>

  <p align="center">
    A Quantum convolution as a first layer intended for feature extraction.
    <br />
    <a href="https://github.com/HectorIGH/Quantum-Convolution"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/HectorIGH/Quantum-Convolution">View Code</a>
    ·
    <a href="https://github.com/HectorIGH/Quantum-Convolution/issues">Report Bug</a>
    ·
    <a href="https://github.com/HectorIGH/Quantum-Convolution/issues">Request Feature</a>
  </p>
</p>



<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

[![Product Name Screen Shot][product-screenshot]](https://hectorigh.github.io/)

There are two base models. 

One is intended to be optimized by Tensorflow. A custom layer is built and custom training and evaluation  loops are created, then the model is optimized. Ideally, Tensorflow would optimize the parameters in the quantum circuit, nevertheless when extracting the numpy array representation from the tensor in order to execute the quantum circuit, the ability of that tensor to be optimized is lost. This model is found in _this [Notebook](https://github.com/HectorIGH/Quantum-Convolution/blob/main/Custom%20Training%20%26%20GradientTape%20for%20Qonv2D%20Initial%20Layer.ipynb)_.

The second model is a compromise with the optimization incapability. Instead, a random set of filters is generated and applied to the original dataset, obtaining the first convolution. Since performing the quantum convolution on the fly is quite slow, the output images are saved into an npy file, which is then loaded and used as the input to a subsecuent classical convnet model. For comparison reasons, a classical model, different only in the first convolution, is implemented. This model can be found in _this [Notebook](https://github.com/HectorIGH/Quantum-Convolution/blob/main/CONVNET%20with%20Quonvolution%20Preprocess.ipynb)_.


### Built With

The model is built in Python and Qiskit for quantum processing. Tensorflow is used for model creation and optimization purposes.

* [Python](https://www.python.org/)
* [Qiskit](https://qiskit.org/)
* [TensorFlow](https://www.tensorflow.org/)



<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

This is an example of how to list things you need to use the software and how to install them.
* npm
  ```sh
  npm install npm@latest -g
  ```

### Installation

1. Get a free API Key at [https://example.com](https://example.com)
2. Clone the repo
   ```sh
   git clone https://github.com/your_username_/Project-Name.git
   ```
3. Install NPM packages
   ```sh
   npm install
   ```
4. Enter your API in `config.js`
   ```JS
   const API_KEY = 'ENTER YOUR API';
   ```



<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://github.com/HectorIGH/Quantum-Convolution/issues)_



<!-- ROADMAP -->
## Roadmap

See the [open issues](https://github.com/HectorIGH/Quantum-Convolution/issues) for a list of proposed features (and known issues).



<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.



<!-- CONTACT -->
## Contact

Héctor Iván García Hernández - [@HectorIGarciaH](https://twitter.com/HectorIGarciaH) - hi.garcia.hdez@gmail.com

Project Link: [https://github.com/HectorIGH/Quantum-Convolution](https://github.com/HectorIGH/Quantum-Convolution)



<!-- ACKNOWLEDGEMENTS -->
<!--
## Acknowledgements
* [GitHub Emoji Cheat Sheet](https://www.webpagefx.com/tools/emoji-cheat-sheet)
* [Img Shields](https://shields.io)
* [Choose an Open Source License](https://choosealicense.com)
* [GitHub Pages](https://pages.github.com)
* [Animate.css](https://daneden.github.io/animate.css)
* [Loaders.css](https://connoratherton.com/loaders)
* [Slick Carousel](https://kenwheeler.github.io/slick)
* [Smooth Scroll](https://github.com/cferdinandi/smooth-scroll)
* [Sticky Kit](http://leafo.net/sticky-kit)
* [JVectorMap](http://jvectormap.com)
* [Font Awesome](https://fontawesome.com)
-->





<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/HectorIGH/Binary-Image-classification-via-QML.svg?style=for-the-badge
[contributors-url]: https://github.com/HectorIGH/Quantum-Convolution/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/HectorIGH/Binary-Image-classification-via-QML.svg?style=for-the-badge
[forks-url]: https://github.com/HectorIGH/Quantum-Convolution/network/members
[stars-shield]: https://img.shields.io/github/stars/HectorIGH/Binary-Image-classification-via-QML.svg?style=for-the-badge
[stars-url]: https://github.com/HectorIGH/Quantum-Convolution/stargazers
[issues-shield]: https://img.shields.io/github/issues/HectorIGH/Binary-Image-classification-via-QML.svg?style=for-the-badge
[issues-url]: https://github.com/HectorIGH/Quantum-Convolution/issues
[license-shield]: https://img.shields.io/github/license/HectorIGH/Binary-Image-classification-via-QML.svg?style=for-the-badge
[license-url]: https://github.com/HectorIGH/Quantum-Convolution/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/hector-ivan-garcia-hernandez
[product-screenshot]: README_images/Qonvolution.svg
