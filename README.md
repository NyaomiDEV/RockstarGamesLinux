# Rockstar Games Linux

Currently featuring support for Grand Theft Auto V but probably other stuff works too.

## Why?

I wanted to play GTA Online and Lutris kept having bugs here and there which I cannot possibly explain, but anyway they resulted in me being basically unable to use the keyboard to play the game and having glitches due to some DXVK issues (I suppose).

## How?

- Clone this repository's files into the correct places (`$HOME`)
- Modify your `config.env` file so that your correct game directory is set (will be mapped to `Z:`)
- Run the Rockstar Games Launcher script and it will automatically set up everything for you (it will take some time though)
- Login and download GTA V (or any other games if they have the same requirements as GTA V) (and possibly on the virtual `Z:` drive).
- Close the Rockstar Games Launcher
- Use the game icon in the apps list to launch GTA V (very important)
- For other games, make your own scripts and contribute to this repo afterwards

Your saves will be located at `$HOME/.local/share/Rockstar Games/Saves/` as per XDG specification.

For the techies out there, the Wine prefix is located by default at `$HOME/.local/share/Rockstar Games/wineprefix/`.

If you plan on playing GTA Five with the keyboard then note that the stock Wine has a bug that makes the game freeze for a few seconds whenever a keyboard input is pressed. I'd be glad to know the root cause of this, but searching on Bugzilla gave me no results.

## Epic Games version?

Y'all have got Legendary and Heroic. Use them.

## Considerations

- At any point you can nuke the Wine prefix because your saves and game are actually saved elsewhere; but remaking it from scratch takes time, so probably don't screw up too much
- If a dependency is missing to run some other game than GTA V (and it doesn't break GTA V itself), feel free to make a pull request
- MangoHud is loaded by default; if you don't want it, simply edit the Rockstar Games script and remove the lines that load it in. Prolly I should put that in `config.env`.
- You've got to own the games on Rockstar Games Social Club to be able to download/play them at all (no game assets are hosted here).
- Cracked versions of the games will not work, and don't ask for support.

## License

I am not responsible for damages you do on your computer, and even in front of a judge in court I will cite the following:

```
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED,
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

## Is this legal?

Well, I am not hosting any game assets except some images that are used for the sole purpose of game/launcher identification in a list of installed applications ("icons"); so I, as the author, am technically in the clear.

Gaming on Linux should also be within the Rockstar Games EULA, provided I have read it and I didn't see anything that contradicts playing those games in OSes other than Windows.

So, for a common understanding, since this project doesn't host important game assets and it doesn't condone piracy nor cheating in any way, shape or formm, we all should be in the clear.

If I am mistaken, I will be glad to remove everything from here. I hope I won't have TT's lawyers knocking at my door tomorrow.
