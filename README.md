[commits]: https://github.com/latte-soft/rdd/commits
[badges/last-modified]: https://img.shields.io/github/last-commit/latte-soft/rdd?label=Last%20Modifed

> [!CAUTION]
> The only *official* host of RDD is [**`rdd.[latte.to]`**](https://rdd.latte.to). Under no circumstances is Latte Softworks responsible for any potential harm caused by using an unofficial fork/rehost of RDD, though anyone is free to fork off of or rehost RDD as it is under the MIT license. RDD is a static website with none of its own backend infrastructure, binaries are fetched directly from Roblox's official content delivery network via [**`setup-aws.[rbxcdn.com]`**](https://setup-aws.rbxcdn.com).

## RDD ("Roblox Deployment Downloader")

[![Last Modified][badges/last-modified]][commits]

Locally download Roblox deployments (Windows/Mac) directly from your browser!

Hosted officially @ <https://rdd.latte.to>

### What is this?

RDD can assemble plain resources directly from Roblox's [`setup`](https://setup.rbxcdn.com) S3 storage bucket into a format the user would expect to be able to directly extract/run from. **Everything is fetched locally in your browser, without any additional required server resources!**

### Usage

```txt

[*] USAGE: https://rdd.latte.to/?channel=<CHANNEL_NAME>&binaryType=<BINARY_TYPE>&version=<VERSION_HASH>

    Binary Types:
    * WindowsPlayer
    * WindowsStudio64
    * MacPlayer
    * MacStudio

    Extra Notes:
    * If `channel` isn't provided, it will default to "LIVE" (the production channel)

    You can also use an extra query argument we provide, `blobDir`, for specifying
    where RDD should fetch deployment files from. This is useful for using different
    relative directories than normal for a certain client type, such as for fetching
    stuff from /mac/arm64/ instead of /mac/

    Blob Directories (Examples):
    * "/" (Default for WindowsPlayer/WindowsStudio64)
    * "/mac/" (Default for MacPlayer/MacStudio)
    * "/mac/arm64/"
    ..
```

### Extras

* [JSZip](https://github.com/Stuk/jszip) (Used for `WindowsPlayer`/`WindowsStudio` file extraction/generation)
* <https://github.com/latte-soft/channel-tracker>

## License

See file: [LICENSE](LICENSE)

```
MIT License

Copyright (c) 2024-2025 Latte Softworks <https://latte.to>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
