# Inconsistent Flexbox Layout with `space-between` and Fixed Width Children

This repository demonstrates a subtle bug in CSS flexbox layout.  The issue arises when using `justify-content: space-between` with child elements that have a fixed width.  The resulting layout is inconsistent across different browsers, due to how browsers handle the space between flex items and the inherent space taken up by the `space-between` property itself. The solution provided adjusts the width of child elements to achieve consistent behavior.

## Bug Description:

The bug demonstrates how using `justify-content: space-between` with child elements having a fixed width can lead to variations in spacing and layout across different browsers. The root cause is that a fixed width doesn't factor in the space already allocated by `space-between` for spacing.

## Solution:

The solution explains how to overcome the problem by accounting for the gaps when setting the width of the child elements, ensuring a consistent layout across browsers.