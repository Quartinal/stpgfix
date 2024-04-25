# stpgfix
fix for the payload generator made by TheMemeSniper for the securly code execution exploit found by bypassi

in the securly for chromebooks (filter) extension, the b64 + urlencoded data for the category field is blindly put on the page, so we can exploit that to run code on these pages. this is utilized by bypassi to stage his point-blank exploit, but can be used for other purposes.

- I added external crates to src/main.rs, just in case this package doesn't work for you guys!

- Whenever you feel ready, run this with:

```shell
cargo run --package stpgfix --bin stpgfix "chrome-extension://iheobagjkfklnlikgihanlhcddjoihkg/blocked.html?category="
```