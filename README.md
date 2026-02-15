# Huffman Encoding in Rust

## Description

This uses near-optimal encoding.

The tree is encoded in-order, as in the leaves are sorted 
left to right. It is encoded in code-length, ascii value form,
with code-length and ascii value both being bytes.

After that it's traditional huffman encoding.

Some space could be saved by removing the first bit from
the ascii values since ascii is only 7 bytes and doing the
same for the length since the tree cannot get longer than 
that for the same reason.

## Usage

From source, make sure you have cargo installed and run

```bash
cargo run -- {file_you_want_encoded} -o {output_file_name}
```
