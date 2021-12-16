## GIFTjs

Lightweight node module for data encryption and decryption using lightweight encryption algorithm GIFT-128.
This is Nodejs adaptation of [GIFT-128 C implementation](https://github.com/giftcipher/gift) for the purpose of its future implementation in IoT.

<!-- ABOUT THE PROJECT -->
## About The Project

GIFT-128-128 is a 40-round SPN cipher, which have a key length of 128-bit.
GIFT is a very simple and clean design that outperforms even SIMON or SKINNY for round-based implementations, making it one of the most
energy efficient ciphers as of today. It reaches a point where almost
the entire implementation area is taken by the storage and the Sboxes,
where any cheaper choice of Sbox would lead to a very weak proposal.
In essence, GIFT is composed of only Sbox and bit-wiring, but its natural
bitslice data flow ensures excellent performances in all scenarios, from
area-optimised hardware implementations to very fast software implementation on high-end platforms.

## Installation

   ```sh
   npm i giftjs
   ```
   
## Usage

Encrypt and decrypt are functions that accept 2 parameters(PLAINTEXT - 128bit hex, KEY - 128bit hex).
Both functions permute PLAINTEXT variable.
```js
import { encrypt , decrypt } from 'giftjs';

encrypt(PLAINTEXT,KEY);
decrypt(PLAINTEXT,KEY);

```


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<!-- CONTACT -->
## Contact

Igor Tomic - itomic41@gmail.com

Project Link: [https://github.com/igortomic99/giftjs.git](https://github.com/igortomic99/giftjs.git)

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [GIFT: A Small Present
Towards Reaching the Limit of Lightweight Encryption](https://eprint.iacr.org/2017/622.pdf)
* [GIFT Ciphers project](https://giftcipher.github.io/gift/)
