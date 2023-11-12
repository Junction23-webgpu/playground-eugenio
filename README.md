# [fantasy-world-generator](https://fantasy-world-generator.euber.dev/)

Fantasy world generator is a proof of concept for the WebGpu API introduced on some browsers, that will slowly replace the webgl one.

## The context

The project was done for the challenge *["veikkaus"](https://www.junction2023.com/challenges-2023/veikkaus)* of **[Junction2023](https://www.junction2023.com/)**

## The purpose

Altough a relative new API, supported (as of now, 12/11/2023) only [by some browsers](https://caniuse.com/webgpu), it will extensibly used in the future. It's a new API, that solves many problems that WebGL has and that has more functionalities and a much greater access to the GPU power. 

The purpose was experimenting with it and being a team of three people that did not know anything about WebGL or these type of libraries, we are very satisfied with our result.

## The project

Our proof of concept generates random worlds, composed of islands and the sea. It consists in only an html file, with all the JS and WSGL code included there. It is remarkable the usage of the **Perlin** algorithm directly in the WSGL code for performance reasons, by still keeping the result non-deterministic. A problem we faced was exatcly the difficulty in realizing random numbers (e.g. with a seed), that we solved by generating the number with Math.random() on JS and binding that var in the WSGL code.

## The demo

Our demo is available at [https://fantasy-world-generator.euber.dev](https://fantasy-world-generator.euber.dev)

A video presentation is available at [https://youtu.be/g6MUypJ0fCc](https://youtu.be/g6MUypJ0fCc)
