# Ex09 Event Registration Web Application
## Date:07.10.2025

## AIM:
To design, develop and deploy a web application for event registration.

## DESIGN STEPS:

### Step 1:
Create a new frame.

### Step 2:
Select any one preset size of your choice.

### Step 3:
Select the shapes you need.

### Step 4:
Import images as needed.

### Step 5:
Create pages based on your need and link them.

### Step 6:

Validate the HTML and CSS code.

### Step 6:

Publish the website in the given URL.

## DESIGN TOOL:
Figma

## CODE:
```
frame 1
import React from "react";
import web11 from "./web1-1.png";
import web12 from "./web1-2.png";

export const Frame = () => {
  return (
    <div className="bg-white w-full min-w-[223px] min-h-[456px] relative">
      <img
        className="top-0 left-0 w-[223px] h-[456px] aspect-[0.67] absolute object-cover"
        alt="Web"
        src={web12}
      />

      <div className="absolute top-[79px] left-5 [font-family:'Inter-Bold',Helvetica] font-bold text-[#1347b8] text-[40px] tracking-[0] leading-[normal] whitespace-nowrap">
        BOOK
      </div>

      <div className="absolute top-[273px] left-[43px] w-[131px] h-10 bg-[#ff82e4]" />

      <div className="absolute top-[284px] left-[72px] w-[93px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#f8161a] text-base tracking-[0] leading-[normal]">
        REGISTER
      </div>

      <div className="absolute top-[134px] left-[62px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#1b1eb8] text-[40px] tracking-[0] leading-[normal] whitespace-nowrap">
        FAIR
      </div>

      <div className="absolute top-[189px] left-[61px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#261aa8] text-[40px] tracking-[0] leading-[normal] whitespace-nowrap">
        EVENTS
      </div>

      <img
        className="top-3 left-[7px] w-[203px] h-[31px] aspect-[6.53] absolute object-cover"
        alt="Web"
        src={web11}
      />
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}


frame 2
import React from "react";
import web21 from "./web2-1.png";

export const Frame = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[230px] min-h-[456px] relative">
      <img
        className="absolute top-0 left-0 w-[230px] h-[456px] aspect-[2.01] object-cover"
        alt="Web"
        src={web21}
      />

      <div className="absolute top-[228px] left-10 [font-family:'Inter-Bold',Helvetica] font-bold text-[#0c187e] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        Literary quiz
      </div>

      <div className="absolute top-[279px] left-10 [font-family:'Inter-Bold',Helvetica] font-bold text-[#0f1c8e] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        Poetry slam
      </div>

      <div className="top-[71px] left-[17px] bg-[#f01414] absolute w-2 h-2 rounded" />

      <div className="absolute top-4 left-[21px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#f43b44] text-xl tracking-[0] leading-[normal] whitespace-nowrap">
        BOOK FAIR EVENTS
      </div>

      <div className="absolute top-[67px] left-10 [font-family:'Inter-Bold',Helvetica] font-bold text-[#1c1192] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        Reading marathon
      </div>

      <div className="top-[93px] -left-4 bg-[#d9d9d9] absolute w-2 h-2 rounded" />

      <div className="top-[121px] left-[17px] bg-[#f3181b] absolute w-2 h-2 rounded" />

      <div className="top-[180px] left-[17px] bg-[#e61a24] absolute w-2 h-2 rounded" />

      <div className="top-[235px] left-[17px] bg-[#fa1e1e] absolute w-2 h-2 rounded" />

      <div className="top-[285px] left-[17px] bg-[#f51515] absolute w-2 h-2 rounded" />

      <div className="absolute top-[117px] left-[39px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#2e119f] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        Story telling sessions
      </div>

      <div className="absolute top-[174px] left-10 [font-family:'Inter-Bold',Helvetica] font-bold text-[#2e1494] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        Book launch corner
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame 3
import React from "react";
import image from "./image.svg";
import textOnAPath2 from "./text-on-a-path-2.svg";
import textOnAPath from "./text-on-a-path.svg";
import web31 from "./web3-1.png";

export const Frame = () => {
  return (
    <div className="bg-white overflow-hidden w-full min-w-[227px] min-h-[456px] relative">
      <img
        className="absolute top-0 left-0 w-[227px] h-[456px] aspect-[0.67] object-cover"
        alt="Web"
        src={web31}
      />

      <div className="absolute top-[11px] left-[29px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#fa485d] text-base tracking-[0] leading-[normal] whitespace-nowrap">
        REGISTRATION FORM
      </div>

      <img
        className="absolute top-[251px] left-[620px] w-[106px] h-[17px]"
        alt="Text on a path"
        src={textOnAPath}
      />

      <img
        className="absolute top-[279px] left-[620px] w-[139px] h-[21px]"
        alt="Text on a path"
        src={image}
      />

      <div className="absolute top-[49px] left-5 w-[116px] h-5 bg-[#d9d9d9]" />

      <div className="absolute top-[157px] left-[21px] w-[147px] h-8 bg-[#d9d9d9]" />

      <div className="absolute top-[164px] left-[29px] [font-family:'Inter-Medium',Helvetica] font-medium text-black text-sm tracking-[0] leading-[normal]">
        Mobile Number
      </div>

      <div className="absolute top-20 left-5 w-[116px] h-[25px] bg-[#d9d9d9]" />

      <div className="absolute top-[82px] left-[31px] [font-family:'Inter-Medium',Helvetica] font-medium text-black text-sm tracking-[0] leading-[normal]">
        Age
      </div>

      <img
        className="absolute top-[329px] left-[611px] w-[135px] h-[26px]"
        alt="Text on a path"
        src={textOnAPath2}
      />

      <div className="absolute top-[116px] left-5 w-[124px] h-[23px] bg-[#d9d9d9]" />

      <div className="absolute top-[119px] left-[29px] [font-family:'Inter-Medium',Helvetica] font-medium text-black text-sm tracking-[0] leading-[normal]">
        Gender
      </div>

      <div className="absolute top-[207px] left-[21px] w-[135px] h-[25px] bg-[#d9d9d9]" />

      <div className="absolute top-[210px] left-[31px] w-[62px] [font-family:'Inter-Medium',Helvetica] font-medium text-black text-sm tracking-[0] leading-[normal]">
        Email Id
      </div>

      <div className="absolute top-[51px] left-[31px] [font-family:'Inter-Medium',Helvetica] font-medium text-black text-sm tracking-[0] leading-[normal]">
        Full Name
      </div>

      <div className="absolute top-[282px] left-[54px] w-[122px] h-[49px] bg-[#ff3fb8]" />

      <div className="absolute top-[293px] left-[58px] w-[118px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#fc172a] text-2xl tracking-[0] leading-[normal]">
        REGISTER
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

frame 4
import React from "react";
import web41 from "./web4-1.png";

export const Frame = () => {
  return (
    <div className="bg-white w-full min-w-[231px] min-h-[456px] relative">
      <img
        className="absolute top-0 left-0 w-[231px] h-[456px] aspect-[0.46] object-cover"
        alt="Web"
        src={web41}
      />

      <div className="absolute top-[54px] left-11 [font-family:'Inter-Bold',Helvetica] font-bold text-[#5b139f] text-4xl tracking-[0] leading-[normal]">
        THANK
      </div>

      <div className="absolute top-[116px] left-[76px] [font-family:'Inter-Bold',Helvetica] font-bold text-[#1810b0] text-4xl tracking-[0] leading-[normal]">
        YOU
      </div>
    </div>
  );
};

/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./src/**/*.{html,js,ts,jsx,tsx}"],
  theme: {
    extend: {},
  },
  plugins: [],
};

@tailwind components;
@tailwind utilities;

@layer components {
  .all-\[unset\] {
    all: unset;
  }
}

:root {
  --animate-spin: spin 1s linear infinite;
}

.animate-fade-in {
  animation: fade-in 1s var(--animation-delay, 0s) ease forwards;
}

.animate-fade-up {
  animation: fade-up 1s var(--animation-delay, 0s) ease forwards;
}

.animate-marquee {
  animation: marquee var(--duration) infinite linear;
}

.animate-marquee-vertical {
  animation: marquee-vertical var(--duration) linear infinite;
}

.animate-shimmer {
  animation: shimmer 8s infinite;
}

.animate-spin {
  animation: var(--animate-spin);
}

@keyframes spin {
  to {
    transform: rotate(1turn);
  }
}

@keyframes image-glow {
  0% {
    opacity: 0;
    animation-timing-function: cubic-bezier(0.74, 0.25, 0.76, 1);
  }

  10% {
    opacity: 0.7;
    animation-timing-function: cubic-bezier(0.12, 0.01, 0.08, 0.99);
  }

  to {
    opacity: 0.4;
  }
}

@keyframes fade-in {
  0% {
    opacity: 0;
    transform: translateY(-10px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes fade-up {
  0% {
    opacity: 0;
    transform: translateY(20px);
  }

  to {
    opacity: 1;
    transform: none;
  }
}

@keyframes shimmer {
  0%,
  90%,
  to {
    background-position: calc(-100% - var(--shimmer-width)) 0;
  }

  30%,
  60% {
    background-position: calc(100% + var(--shimmer-width)) 0;
  }
}

@keyframes marquee {
  0% {
    transform: translate(0);
  }

  to {
    transform: translateX(calc(-100% - var(--gap)));
  }
}

@keyframes marquee-vertical {
  0% {
    transform: translateY(0);
  }

  to {
    transform: translateY(calc(-100% - var(--gap)));
  }
}

```
## OUTPUT:
![alt text](<Screenshot 2025-10-07 152716.png>)

## RESULT:
The program to design, develop and deploy a web application for event registration is completed successfully.
