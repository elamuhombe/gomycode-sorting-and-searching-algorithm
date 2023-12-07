# Insertion Sort Algorithm

## Overview

This repository contains a simple implementation of the insertion sort algorithm in pseudocode. The insertion sort algorithm is a straightforward sorting algorithm that builds the final sorted array one item at a time.

## Algorithm Details

The provided pseudocode (`insertion_sort`) demonstrates the insertion sort algorithm. It initializes variables, iterates through the array, and performs the necessary comparisons and swaps to sort the array in ascending order.

## Pseudocode

```plaintext
ALGORITHM insertion_sort
VAR
    arr: ARRAY_OF_INTEGER;
    i, j, temp: INTEGER;

BEGIN
    i := 0;
    j := 0;

    FOR i := 1 TO LENGTH(arr) - 1 DO
        temp := arr[i];
        j := i - 1;

        WHILE j >= 0 AND arr[j] > temp DO
            arr[j + 1] := arr[j];
            j := j - 1;
        END WHILE

        arr[j + 1] := temp;
    END FOR
END
