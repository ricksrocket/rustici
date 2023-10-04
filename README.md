# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

# Rustici App

## Table of Contents

- [Introduction](#introduction)
- [Problem Statement](#problem-statement)
- [Key Features](#key-features)
- [Time Complexity Analysis](#time-complexity-analysis)
- [Usage](#usage)
- [Installation](#installation)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Rustici App is a web-based system designed to deliver randomized tests with multiple-choice questions and randomized answer orders to learners. This README provides an overview of the project, explains the problem statement, outlines key features, and provides instructions for usage and contribution.

## Problem Statement

The client requested a solution to deliver tests with randomized questions and answer orders. The specific requirements were:

- Questions must be presented in a random order each time a learner attempts the test.
- The order of answer choices within each question must also be randomized.
- The system should handle a large number of tests and questions.
- The codebase should be maintainable and work across modern browsers.

## Key Features

### 1. Randomized Questions

- The `shuffleQuestions` function shuffles the order of questions each time it's called.
- It uses the Fisher-Yates Shuffle Algorithm to achieve randomization.

### 2. Randomized Answer Choices

- For each question, the code preserves the original answers' order while randomizing the order of answer choices.
- This ensures that the correct answers remain consistent.

### 3. Scalability

- The code is designed to handle a large number of tests and questions efficiently.
- It can support tests with up to 20 questions, each with up to 6 answer choices.

## Time Complexity Analysis

The key feature, shuffling questions and answer choices, involves the Fisher-Yates Shuffle Algorithm. The time complexity of this algorithm is O(n), where n is the number of elements to be shuffled. In this app, the number of questions and answer choices determines the value of n.

## Usage

1. Clone the repository to your local machine.
2. Install the necessary dependencies using `npm install`.
3. Run the app using `npm start`.
4. Click the "Shuffle Questions" button to randomize the question order and answer choices.

## Installation

To run this app locally, you need to have Node.js and npm (Node Package Manager) installed on your system. Follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/rustici-app.git
