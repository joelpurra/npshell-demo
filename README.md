<p align="center">
  <a href="https://github.com/joelpurra/npshell/"><img src="https://cloud.githubusercontent.com/assets/1398544/5836151/b8d8e31e-a171-11e4-8412-d23765b54a25.gif" alt="npshell in action" border="0" /></a>
</p>


# [npshell `np`](https://github.com/joelpurra/npshell/) [demo code](https://github.com/joelpurra/npshell-demo/)

Automate demo creation, showing [`np`](https://github.com/joelpurra/npshell/) music player commands in action.


## Usage



### Dummy files

`np` won't play empty files, so they all need to be replaced with a `dummy.mp3` file 30 seconds long or so. Didn't include one in this repository, so pick one yourself.

1. Replace the empty placeholder files in this repository with a `dummy.mp3` file using the command below.
1. Put the dummy files in `~/Music`, which shouldn't contain any other files during the demo.

```bash
find . -type f -name '*.mp3' -print0 | xargs -0 -I '{}' cp "dummy.mp3" "{}"
```



### Recording demo

Using [`shell-keystroke-animator`](https://github.com/joelpurra/shell-keystroke-animator).

1. Open two terminal windows.
1. In the first, enter the below command.
1. Switch to the second window.
1. Let the commands complete before doing anything else.
1. Use the resulting `ouput.gif`.

```bash
cat "steps.sh" | keystroke-animator
```



## Kudos

- [Elisabeth Nilsson](https://www.grisenskriker.se/) and [Måns Jonasson](https://mansjonasson.se/) for a broad album selection.
- [Wikipedia](https://www.wikipedia.org/) for track listings.



---

Copyright (c) 2015, 2016 [Joel Purra](https://joelpurra.com/). Released under [GNU General Public License version 3.0 (GPL-3.0)](https://www.gnu.org/licenses/gpl.html).
