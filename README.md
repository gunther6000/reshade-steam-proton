# reshade-linux
Bash script to download ReShade and the shaders and link them to games running with wine or proton on Linux.  

## Usage

### Quick:
Download the script:

    curl -LO https://github.com/kevinlekiller/reshade-steam-proton/raw/main/reshade-linux.sh
Make it executable:

    chmod u+x reshade-linux.sh
Execute the script:

    ./reshade-linux.sh

### Detailed:
For detailed usage, follow the instructions in the script's source:

https://github.com/kevinlekiller/reshade-steam-proton/blob/main/reshade-linux.sh#L21

## Alternatives
Currently a bit more limited, so some effects will not work. Depending on your needs, the options below may be more performant.

### vkBasalt:
https://github.com/DadSchoorse/vkBasalt

For native Linux Vulkan games, Windows games which can run through DXVK (D3D9 / D3D10 / D3D11) and Windows games which can run through VKD3D (D3D12). 

### gamescope:

Since 3.12.6, [gamescope](https://github.com/ValveSoftware/gamescope) supports a subset of Reshade effects/shaders using the `--reshade-effect [path]` and `--reshade-technique-idx [idx]` command line parameters.

### vkBasalt through gamescope:

Since gamescope can use Vulkan, you can run vkBasalt on gamescope itself, instead of on the game.
