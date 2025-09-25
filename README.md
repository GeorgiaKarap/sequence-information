# Sequence Information
This repository contains three C programs for analyzing DNA and protein sequences:

- GC content.c<br>
Calculates the GC content (%) of a DNA sequence.</p>

- maximum length.c<br>
Finds the maximum length among multiple sequences.</p>

- sequence length.c<br>
Computes the lengths of two sequences and identifies the longer one.</p>

---

## Features

- Compute GC content of DNA sequences from an input file.
- Find maximum sequence length in a file.
- Compare two sequences of different files and identify the longer one.
- Simple, fast, and file-based input handling.

---

## Project Structure

- .gitignore
- content
  - GC content.c
  - dna.seq
- LICENSE
- README.md
- length
  - maximum length.c
  - seq.dat
  - seq2.dat
  - sequence length.c

---

## How It Works

The programs read sequences from input files (dna.seq, seq.dat).
Each program performs a specific analysis:<br>
GC content: Counts G and C nucleotides and calculates the percentage.<br>
Maximum length: Scans all sequences to find the longest one.<br>
Sequence length: Measures each sequence’s length and compares them.<br>
Results are printed directly to the console.

---

## Example Usage

- GC Content<br>
./gc_content < dna.seq</p>
Output example:<br>
The %GC is 61.596958

- Maximum Length<br>
./maximum_length < seq.dat </p>
Output example:<br>
The Maximum length is 108

- Sequence Length<br>
cat seq.dat seq2.dat | ./sequence_length</p>
Output example:<br>
The length of the first sequence is 188<br>
The length of the second sequence is 80<br>
The Maximum is 118

---

## Input Files

- dna.seq: DNA sequences (characters: A, T, G, C)<br>
- seq.dat: Protein sequences
- seq2.dat: Protein sequences

---

## Installation

Download the zip file and unzip it.<br>
For the GC content program open the terminal and go to the "content" file.<br>
For sequence length and maximum length programs go to the "length" file.


---

## Compilation

Compile each program with gcc as follows:

- Compile GC Content program<br>
gcc -o gc_content "GC content.c"</p>

- Compile Maximum Length program<br>
gcc -o maximum_length "maximum length.c"</p>

- Compile Sequence Length program<br>
gcc -o sequence_length "sequence length.c"</p>

This will create executable files: gc_content, maximum_length, and sequence_length.

---

## Execution

Run each program using the compiled executable and provide the input file:

- Run GC Content<br>
./gc_content < dna.seq

- Run Maximum Length<br>
./maximum_length < seq.dat

- Run Sequence Length<br>
cat seq.dat seq2.dat | ./sequence_length</p>

Each program read the sequences from standard input and print results to standard output.

---

## Notes

- Supports sequences up to 5000 characters.
- Input files must contain only valid DNA (A, T, G, C) or protein characters.
- For the program "maximum length" the input file must contain one sequence per line without spaces
- The program "sequence length" compares only 2 sequences from 2 different files
- The program "maximum length" compares many sequences located on different lines of the same file

---

## License
This project is licensed under the ΜΙΤ License
