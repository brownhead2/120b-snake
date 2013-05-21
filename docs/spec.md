# Snake and Mouse

I will create the classic game of snake where the player controls the snake via a USB mouse. The game will be displayed on an LED matrix.

## Rules

The player will eat circles on the board that make it larger and receive points on the amount of circles they can eat without dying.

The head of the snake will be entirely controlled by the mouse such that if the mouse is not moving, the snake does not move either. The player cannot move diagonally.

## Possible Features

 1. Keeping score on an LCD. This screen will also serve as a debug console.
 1. Interfacing with USB devices (ie: being able to communicate with the mouse at all).
 1. Controlling the game via a mouse.
 1. Having circles appear on the board randomly that the snake can eat.
 1. The game world is represented on an LED matrix.
 1. Angry and happy messages/displays for losses and wins, respectively.
 1. Heuristics to make sense of the data read from the mouse.
 1. Interface to pause, start, and end the game (some kind of menu).
 1. Having the snake get bigger according to the typical rules of snake.
 1. Keeping the game fun to play despite having to use a mouse to control the snake.

## Project Plan

### "C" Check Off

Implement Snake with the LED Matrix that uses the keypad to control the Snake. The score is displayed on the LCD.

### "B" Check Off

Implement a USB mouse driver such that meaningful information can be read in from the mouse. This can be done by making a dot move around the LED matrix, or displaying coordinates read in from the mouse onto the LCD.

### "A" Check Off

Bring the two projects together and make the Snake game driven by the USB mouse.

## Hardware

I will need a couple pieces of additional hardware for this project: an LED matrix and a USB mouse. I am not sure which model LED matrix I will be using as I am trying to find someone to get it from second-hand, I am also not sure how many pins I will have to devote to the USB protocol. I think I may be able to get away with using only 1 pin, but I haven't delved far enough into the USB spec yet. Therefore the following table is scarce of information.

| Pins           | Device        |
| -------------- | ------------- |
| A[0:3]         | LCD           |
| B[?:?]         | LED Matrix    |
| C[?:?]         | USB Interface |

As can be seen, my hardware needs will be simple. The main issues I will run into are likely to be in software (implementing the USB protocol and creating a suitable mouse driver).
