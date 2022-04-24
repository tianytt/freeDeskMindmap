### Software introduction 

The desktop version of Mind Mapping is a localized version of Baidu Mind Mapping, which helps you to use Mind Mapping Tool without Internet.

### Special Sponsors

<p align="center"><a href="https://documentnode.io/?utm_source=github&utm_medium=sponsor&utm_campaign=desktopnaotu" target="_blank" rel="noopener noreferrer"><img src="https://user-images.githubusercontent.com/2252451/65103852-16463380-da02-11e9-8b58-bea4a84c2e31.png" alt="Document Node logo"></a><br>
Open Document Node, Inspiration Unfold</p>

### How to download

- Method 1：Download through [**Baidu Cloud**](http://pan.baidu.com/s/1jHNBL7C)
- Method 2：Download through [**Github's Releases**](https://github.com/NaoTu/DesktopNaotu/releases)

### System corresponding to each version

| Operating System | Bit | Corresponding File | Size | Support |
| --------  | -----: | -----: | :----  | -- |
| MacOS | 64 bit | DesktopNaotu - macOS - x64 | < 50M | Supports all functions |
| Linux | 64 bit | DesktopNaotu-linux-x64 | < 50M | Supports all functions |
| Windows 7/10 | 64 bit | DesktopNaotu-win32-x64 | < 50M | Supports all functions |
| Windows 7/10 | 32 bits | DesktopNaotu-win32-ia32 | < 50M | Supports all functions |
| Windows XP | 32 bits | DesktopNaotu-Windows-mini | < 8M | Debugging is not supported |

### Functional characteristics

- Basic functions of Baidu Mind Mapping
- Operation of local km files
- Support dragging open km files
- Support association to open km files
- Support for automatic saving
- [Provide **Baidu Mind Mapping** File Download Method](doc/Help.md)
- [Provide **ProcessOn** Mind Map Download Method](doc/Help.md)
- [View Historical Version](doc/History.md)

### Software screenshots

- Windows screenshot

![Windows](screenshot/Windows-en.png)

- Mac OS X screenshot

![OS X](screenshot/OSX.png)

- Linux screenshot

![Linux](screenshot/Linux.png)

### How to compile

#### 1. Install dependencies

```bash
# Install prerequisites
npm install -g gulp
npm install -g bower

# Install dependencies
npm install
bower install
```

#### 2. Change graceful-fs version (For Node `v10.x` or newer)

```bash
npm install graceful-fs

# If error "ReferenceError: primordials is not defined" still occurs, remove the old edition installed by cnpm
rm -rf node_modules/_graceful-fs@3.0.12@graceful-fs

# If a submodule relies on old graceful-fs, please follow the log, locate to its directory, 
# then manually update
cd node_modules/<PATH_TO_MODULE_USING_DEPRECATED_GRACEFUL_FS>
npm install graceful-fs@4.x
```

#### 3. Change `@types/node` to v12.x

```bash
npm install @types/node@12.x
```

#### 4. Build

```bash
gulp
```

#### 5. Try running

```bash
npm run demo
```

### Contact us

Questions and suggestion feedback:

- [Github issues](https://github.com/NaoTu/DesktopNaotu/issues)
- [Join the discussion group](https://gitter.im/DesktopNaotu/DesktopNaotu)
- QQ group：330722928

### License

Code released under the [GPL-2.0 License](LICENSE).
