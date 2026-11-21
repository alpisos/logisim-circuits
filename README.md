# Logisim Circuits

Digital logic circuits built in [Logisim-evolution](https://github.com/logisim-evolution/logisim-evolution).

![4-bit adder](images/4bit-adder-main.png)

## Opening the circuits

1. Install **Logisim-evolution v5.0.0 or newer**.
2. Download a `.circ` file from [`circuits/`](circuits/).
3. In Logisim-evolution: **File → Open**.

> These files were made with Logisim-evolution. The original Logisim 2.7 may not open them.

## Circuits

| Circuit | Description | Sub-circuits |
|---|---|---|
| [4-bit adder](circuits/4bit-adder.circ) | Ripple-carry adder | `my_xor`, `my_and`, `half_adder`, `full_adder` |

## 4-bit adder

Built from the ground up:

- **`my_xor`, `my_and`**: hand-built gates
- **`half_adder`**: adds two bits, outputs sum and carry
- **`full_adder`**: adds two bits plus a carry-in (two half adders)
- **`main`**: four full adders chained together, each carry-out feeding the next carry-in

Set inputs A and B (4 bits each) and read the sum on the output pins, with the final carry-out as the fifth bit.

## License

[MIT](LICENSE)
