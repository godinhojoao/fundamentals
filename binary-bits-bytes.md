# Binary, Bits, Bytes, Kilobytes, Megabytes, and Gigabytes

## Overview

- In this article we will better understand the smallest part of computers: bits.
- Understand why binary, bits, and bytes matter.

- ### Questions

  - Do you know what binary is?
  - Do you know what a bit and a byte are?
  - When developing something that involves colors and utilizes RGB, do you know why we are restricted to a range of 0 to 255 for each color's intensity?

- We will answer each of these questions in this article, let's see it together!

## Binary: What is it?

- Binary is a way of counting and expressing numbers using only two digits: 0 and 1. In the decimal system, we use ten digits (0 through 9), but computers like using binary because it's easy to represent with electronic switches that can either be on (1) or off (0).
- It is needed because computers communicate using transistors, you can learn more here about computers [clicking here](./how-computer-works.md).
  - In short, binary is a way for computers to talk using only 0s and 1s, which makes it simpler for them to process information with electronic switches.
  - You will also hear about it as 'base 2,' which is used by computers. Humans, on the other hand, use base 10 numbers (0 to 9).

## Bits and bytes

- ### Bit

  - Bit is a short for binary digit.
  - Bits are the smallest form of data, basically like an on off switch. It can represent just 0 or 1. Where 0 is related to (low, off, false, etc...) and 1 means (high, on, true, etc..).
  - Typically, when talking about how fast computers communicate or operate, we use **"bits per second" (bps)**.

- ### Byte

  - With 8 Bits we have 1 Byte.
  - With one Byte we are able to represent 1 text character, for example: a.
  - When figuring out how much data a storage device can hold, we use **"bytes"**.

## Bits, Bytes, Kilobytes, Megabytes and Gigabytes

- As you already mentioned bits and bytes are too small, and even a simple file with some characters would need more than 1 byte. So because of that we need these prefixes to "simplify" when we need to talk about large data.
- Bit: 0 or 1 (2 possible values)
- Byte: 8 bits, 2^8 (256 possible values)
- KILObyte: 2^10 bytes -> 1024 bytes
- MEGAbyte: About 1000 Kilobytes (or about 1 million bytes)
- GIGAbyte: About 1000 megabytes (or about 1 billion bytes)

## When working with RGB, why is the color intensity limited to the range of 0 to 255?

- In Cascading Style Sheets (CSS), for example, we use an 8-bit color channel.
  - As you already saw, for each bit we have two possible values: 0 or 1.
  - With 8 bits we have, 2^8 possible values. Or 256 color's intensity levels, ranging from 0 to 255.
- This is why you often encounter the range of 0 to 255 when working with RGB colors in computer graphics and digital imaging. Each of the red, green, and blue channels can independently take on any value in this range, allowing for a wide variety of colors to be represented.

## Difference between 8bit, 16bit, 32bit, and 64bit

- These terms refer to the number of bits that can be processed or transmitted in a single data element.
- As the bit size increases, so does the addressable memory space and the ability to process larger chunks of data in a single operation.
  - This results in increased processing power and memory capacity

## References

- [StanfordOnline CSX0001 - Computer Science 101](https://learning.edx.org/course/course-v1:StanfordOnline+CSX0001+1T2020/home)
- [Techtarget - What is binary?](https://www.techtarget.com/whatis/definition/binary)
- [Youtube - Binary Explained in 01100100 Seconds](https://www.youtube.com/watch?v=zDNaUi2cjv4&ab_channel=Fireship)
- [Youtube - Bits vs Bytes as Fast As Possible](https://www.youtube.com/watch?v=Dnd28lQHquU&ab_channel=Techquickie)
- [Youtube - Bit and Byte Explained in 6 Minutes - What Are Bytes and Bits?](https://www.youtube.com/watch?v=y45v5SLjxaM&ab_channel=HoomanMardox)
- [Youtube - See How Computers Add Numbers In One Lesson](https://www.youtube.com/watch?v=VBDoT8o4q00&ab_channel=InOneLesson)
