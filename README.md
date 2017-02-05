# A Hugo Template for course material

## Site wide configuration

    [params]
    useSQL = true

## Features:

### Column splitting

    [!](columns 6:2:2:2)

    [!](split)

    [!](split note)


### Side note

Embed it in a blockquote:

    > [!](note)
    > My message here


Another way of using it:

    <img ...>

    [!](note) This is a nice image.


### Code

    ```{python nu sm clipboard template}
    for i in range(__iteration__):
        __do_something__
    ```

where we have:

- `nu`: line numbering
- `sm`: small font
- `clipboard`: copy button
- `template`: all variables of the form `__name__` will be formatted specially.

### Secton separator:

    [!](---)
    [!](***)
    [!](&&&)

### Spacing of lists:

    - first
    - second
    - third
    - [!](comfort)    // or [!](comfortable)

### Make a section a highlighted coverpage

    # Section here

    [!](highlight)

    ...

### Make a section vertical aligned to center

    # Section here
    
    [!](middle)

    ...

### Making a box

    > [!](box)
    >
    > ...

or just embed box command in a paragraph.

    This is in a box.  [!](box)

### Embed multi-page PDF

    <div pdf="url-to-pdf" scale="1.0"></div>

### Scale the whole slide

    [!](scale 0.80)


### Image animation

    <div class="slide-show">
        <... class="fragment" />
        ...
    </div>
