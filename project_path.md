# short_put_scanner

    - These repo show how works rust coverage inside MS Vscode 
    using the expansion coverage-gutters
    - a rocky road  

> [!TIP]
> GITHUB Basic writing and formatting syntax [![alt text][1]](https://docs.github.com/en/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
<!-- -->  
> [!TIP]
> Comments Inside JSON – Commenting in a JSON File [![alt text][1]](https://www.freecodecamp.org/news/comments-in-json/)
<!-- -->
> [!TIP]
><!--- THis empty line is necessary for correct format -->
> - Image as link text for a markdown link [![alt text][1]](https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link)
>
> - Whats the recommended syntax for an image with a link? [![alt text][1]][2]
><!--- THis empty line is necessary for correct format -->
>```text <!-- markdownlint-disable-line code-block-style -->
>[![alt text][1]](https://stackoverflow.com/questions/22697688/how-to-cat-eof-a-file-containing-code)
>```
<!--
[1]: ./img/link_symbol.svg
-->
[2]: https://meta.stackexchange.com/questions/2133/whats-the-recommended-syntax-for-an-image-with-a-link
><!--- THis empty line is necessary for correct format -->
<!-- -->

<!-- 
Markdown Preview Github Styling
GitHub Markdown Preview /w markdown list and other add ones
-->

## Start Date of project

```bash <!-- markdownlint-disable-line code-block-style -->
$ date
Mon Jun  2 09:38:12 AM CEST 2025
```

## OS-Version

```bash <!-- markdownlint-disable-line code-block-style -->
$ uname -a
Linux debian 6.1.0-28-amd64 #1 SMP PREEMPT_DYNAMIC Debian 6.1.119-1 (2024-11-22) x86_64 GNU/Linux
```

## Create for your own project a project folder in the Linux console (terminal ,bash shell), e.g. in your your own home directory, and then open this folder as a new project in the MS VSCODE program

<!-- FIXIT add a variable for project name-->

```bash <!-- markdownlint-disable-line code-block-style -->
# cd && mkdir <project_name folder> && cd $_
# command 'cd' change to home folder from logged in user
cd && mkdir rust-example-cov && cd $_ 
```
<!-- -->
>[!TIP]
> Don't forget to save your project on GitHub - saves you serious headaches
<!-- -->
## Init a new rust based project inside the previously generated folder
<!-- -->
```bash <!-- markdownlint-disable-line code-block-style -->
touch README.md \
&& ln -s README.md README \
&& cargo init "." \
&& cargo add rustfmt \
&& rustup component add rustfmt \
&& mkdir examples \
&& cp src/main.rs examples/example.rs \
&& sed -i -e 's/world/example/g' examples/example.rs \
&& rustup  show \
&& rustup  check \
&& rustup toolchain uninstall stable \
&& rustup toolchain install stable \
&& rustup update  --force \
&& rustup show \
&& mkdir tests
```
<!-- NEXT_TASK copy link symbol from another repo via cmd line command-->
<!-- NEXT_TASK workspace_settings create settings.json add copy cSpell.words to it>
<!-- -->
>[!TIP]
> How to cat ```<<EOF>>``` a file containing code
> Test link image for a Markdown link text [![alt text][1]](https://stackoverflow.com/questions/22697688/how-to-cat-eof-a-file-containing-code)
>
><!--- THis empty line inside the block is necessary for correct format -->
<!-- -->
> [!NOTE]
> Run the bash script for generate the testcase inside a normal terminal - not MS VSCODE terminal
><!--- THis empty line is necessary for correct format -->
<!-- -->
> [!TIP]
> Difference between Terminal, Shell and Bash [![alt text][1]](https://medium.com/@krish.raghuram/terminal-shell-and-bash-3e76218c8865)
>
> - The ***terminal*** is the GUI window that you see
> on the screen. It takes commands and shows output.
>
> - The **shell** is the software that interprets and
> executes the various commands that we type in the
> terminal.
>
> - The ***Bash*** (Bourne-again SHell) Shell is a particular shell.
> It stands > for Bourne Again Shell. Some other examples of shell
> are
>
>   - zsh
>
>     Zsh is a shell designed for interactive
>     use, although it is also a powerful
>     scripting language
>
> - bash
>     bourne shell default shell for most
>     Linux/Unix based system
>
> - csh(c shell)
> - tcsh(turbo c shell)
>
> ***CLI(Command Line Interface)*** refers to a user interface in
> computers where users type in commands and see the results
> printed on the screen.

<!-- Link sign - Don't Found a better way :-( - You know a better method? - send me a email -->
[1]: ./img/link_symbol.svg
