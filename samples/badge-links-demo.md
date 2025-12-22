# Badge Link Test

> This document tests various ways to display badge links in markdown when opened in **MarkView**.

Test whether badge images stay on same line or break.

## Test 1: All badges on separate lines (as in your example)

[![NPM](https://img.shields.io/npm/v/mermaid)](https://www.npmjs.com/package/mermaid)
[![Build CI Status](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml/badge.svg)](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml)
[![npm minified gzipped bundle size](https://img.shields.io/bundlephobia/minzip/mermaid)](https://bundlephobia.com/package/mermaid)

## Test 2: All badges on one line

[![NPM](https://img.shields.io/npm/v/mermaid)](https://www.npmjs.com/package/mermaid) [![Build CI Status](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml/badge.svg)](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml) [![npm minified gzipped bundle size](https://img.shields.io/bundlephobia/minzip/mermaid)](https://bundlephobia.com/package/mermaid)

## Test 3: Using HTML line breaks

[![NPM](https://img.shields.io/npm/v/mermaid)](https://www.npmjs.com/package/mermaid)<br>
[![Build CI Status](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml/badge.svg)](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml)<br>
[![npm minified gzipped bundle size](https://img.shields.io/bundlephobia/minzip/mermaid)](https://bundlephobia.com/package/mermaid)

## Test 4: With trailing spaces (hard breaks)

[![NPM](https://img.shields.io/npm/v/mermaid)](https://www.npmjs.com/package/mermaid)  
[![Build CI Status](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml/badge.svg)](https://github.com/mermaid-js/mermaid/actions/workflows/build.yml)  
[![npm minified gzipped bundle size](https://img.shields.io/bundlephobia/minzip/mermaid)](https://bundlephobia.com/package/mermaid)
