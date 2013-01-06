## Overview

A demonstration of the HyperLogLog algorithm given by <authors>[1]. The demo
returns the number of distinct words, reading up to 100 characters in a single
word.

## Setup

    make

## Options

* -f the file to estimate on, if this is not set, then read from stdin
* -k use 2^k buckets
* -s seed value for Murmur3

## Example usage

Using a file:

    ./hll -k 12 -s 44 -f somefile

Or reading from stdin:

    cat somefile | ./hll -k 12 -s 44