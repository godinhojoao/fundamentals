# Base64 Encoding

## Overview

- In this article we will understand more about Base64 encoding and the importance of knowing this content.
- If you are here, reading this article, probably you know the advantages of knowing Computer Science fundamental contents, right?
  - So, I will save your time, and let's learn more about Base64 encoding and why it is used.
- This article is for those who already used Base64 when programming but have no idea about what heck is it and how it works.

## What is it?

- Base64 is a way of transforming any data into a mnix of digits and letters.
  - Sometimes we just use it because there is no choice. In some situations, only such text-like is considered valid.
- It is a binary-to-text algorithm used to convert data as plain text.
- Given the high popularity of the algorithm, Base64 is well documented, is supported by various programming languages.

- ### How it works?

  - The encoding algorithm of Base64 takes as an input one binary sequence and ouputs another binary sequence. It only gets the binary, splits it into chunks of 6 bits and converts every chunk into a character (a binary sequence that represents this character).
  - So with Base64 encoding we are able to convert any data into a "readable" string just by replacing "6 digits" (6 bits) with one "leter". And as this has a "pattern" we are able to decode this "text" and see it's data, for example, an image.
    - To realize the difference, check out a 5x5 image converted to binary digits:
      `010001 110100 100101 000110 001110 000011 011101 100001 000000 010000 000000 000001 000000 001111 000000 000000 000000 001111 111100 000000 000000 000000 000000 000000 000000 000010 110000 000000 000000 000000 000000 000000 000000 010000 000000 000001 000000 000000 000000 000010 000000 100100 010000 000001 000000 000011 001011`
    - Although the same image converted to Base64 looks like this: `R0lGODdhAQABAPAAAP8AAAAAACwAAAAAAQABAAACAkQBADs`
    - The difference is obvious, even if you remove spaces or padding zeros from binary digits, the Base64 string will still be shorter.

- ### Base64 Characters

  - Base64 Alphabet contains 64 basic ASCII characters which are used to encode data. Yes, with 64 characters we are able to encode data of any length. All these symbols are available in 7-bit and 8-bit character sets, the original ASCII was a 7-bit set with 128 possible characters.
  - Base64 letters are case sensitive, when decoding "QQ==", and "Qq==" the results are different.

- ### What are the padding characters?

  - The equal sign (=) is used for padding and it is always appended at the end of the output. This padding character ensures that the length of Base64 value is a multiple of 4 bytes.
    - The equal sign is not considered part of the encoded data in Base64.
    - Only indexes determine which characters will be used to encode the data. All indexes are listed in the Base64 table.
  - This padding character is needed because of how Base64 works.
    - In the Base64 encoding scheme, each three bytes (24 bits) of binary data are represented by four Base64 characters (6 bits = 1 base64 char -> 6\*4 = 24).
    - If the length of the binary data is not a multiple of 3, padding is added to make it so.

- ### Memory usage issue

  - It makes data about 33% larger in terms of memory usage. Base64 is one of the things that can make software slow.
    - Example:
      - “ABC” (Length = 3) to Base64, the result is “QUJD” (Length = 4)
      - That is, the result is approximately 33% (more exactly, 4/3) larger than the original data.
    - This is why we need to use it only if really necessary. This is the reason to understand better about this encoding and how it works, in this way you will be able to use it correctly.

## Why is it necessary and used for? And when avoiding using it?

- ### When is it necessary?

  - This is widely used to encode binary data (images, sound files)
    - Save binary files to database when BLOB is unavailable
  - In order to prevent data corruption during transmission between different storage mediums.
    - Preserve raw bytes of cryptographic functions
  - To embed binary data into text documents such as HTML, CSS, JavaScript, or XML.
    - Attach files on email
    - Embed images in HTML or CSS via data URI

- ### When avoiding using it?

  - As Base64 is an encoding used to convert data into a "realible" format to ensure that it will not be damaged during transmission we can't use it for another reasons such as encrypting passwords.
  - [Base64 encryption is a lie](https://base64.guru/blog/base64-encryption-is-a-lie), in this article you will see that a lot of developers who don't know when using Base64 were using to "encrypt" passwords, but this is totally wrong as you already know anyone can decode a Base64.
    - This article also provides you the difference between: **encryption, encoding and hashing**.

## References

- [Base64 guru](https://Base64.guru/)
- [freecodecamp what is Base64 encoding](https://www.freecodecamp.org/news/what-is-Base64-encoding/)
- [stack overflow what is Base64 used for?](https://stackoverflow.com/questions/201479/what-is-base-64-encoding-used-for)
- [builtin Base64 encoding](https://builtin.com/software-engineering-perspectives/Base64-encoding)
- [stack overflow Base64 padding character](https://stackoverflow.com/questions/4080988/why-does-Base64-encoding-require-padding-if-the-input-length-is-not-divisible-by)
- [Data URLs MDN web docs](https://developer.mozilla.org/en-US/docs/Web/HTTP/Basics_of_HTTP/Data_URLs)

## Thanks for Reading!

- Feel free to reach out if you have any questions, feedback, or suggestions. Your engagement is appreciated!

## Contacts

- You can find this and more content on:
  - [GitHub](https://github.com/godinhojoao)
  - [LinkedIn](https://www.linkedin.com/in/joaogodinhoo/)
  - [Dev Community](https://dev.to/godinhojoao)
