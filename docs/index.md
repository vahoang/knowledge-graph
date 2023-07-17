# Welcome

Sharing stuffs.

## How to contribute

This page is powered by [mkdocs.org](https://www.mkdocs.org) and using [mkdocs material](https://squidfunk.github.io/mkdocs-material/).

To contribute kindly clone the [repo](https://github.com/vahoang/knowledge-graph), read the template document [here](https://squidfunk.github.io/mkdocs-material/getting-started/) and add new pages by creating PR.

## Mkdocs Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.

## Some sample components

### Tabs

=== "Sample Tab 1"
    Markdown **content**.

    Multiple paragraphs.

=== "Sample Tab 2"
    More Markdown **content**.

    - list item a
    - list item b

### Content Tabs with code blocks

!!! example

    === "C"
    ``` c
    #include <stdio.h>

    int main(void) {
      printf("Hello world!\n");
      return 0;
    }
    ```

    === "C++"
    ``` c++
    #include <iostream>

    int main(void) {
      std::cout << "Hello world!" << std::endl;
      return 0;
    }
    ```

    === "Python"
    ``` py title="bubble_sort.py"
    def bubble_sort(items):
        for i in range(len(items)):
            for j in range(len(items) - 1 - i):
                if items[j] > items[j + 1]:
                    items[j], items[j + 1] = items[j + 1], items[j]
    ```

### Diagrams

#### Flowchart

``` mermaid
graph LR
  A[Start] --> B{Error?};
  B -->|Yes| C[Hmm...];
  C --> D[Debug];
  D --> B;
  B ---->|No| E[Yay!];
```

#### Sequence diagram

``` mermaid
sequenceDiagram
  autonumber
  Alice->>John: Hello John, how are you?
  loop Healthcheck
      John->>John: Fight against hypochondria
  end
  Note right of John: Rational thoughts!
  John-->>Alice: Great!
  John->>Bob: How about you?
  Bob-->>John: Jolly good!
```
