# webcmd-plugin-nasa-images

NASA Images commands for Webcmd.

## Install

```bash
# From local development directory
webcmd plugin install file:///Users/rishabh/Developer/clis/webcmd-plugin-nasa-images

# From GitHub
webcmd plugin install github:rishabhraj36/webcmd-plugin-nasa-images
```

## Commands

| Command | Type | Description |
|---------|------|-------------|
| `nasa-images/search` | JavaScript | Search NASA Images and Video Library media |
| `nasa-images/asset` | JavaScript | List downloadable asset files for a NASA media item |
| `nasa-images/metadata` | JavaScript | Get the metadata JSON URL for a NASA media item |
| `nasa-images/captions` | JavaScript | Get the caption file URL for a NASA video item |

## Examples

```bash
webcmd nasa-images search "apollo 11" --limit 3 -f json
webcmd nasa-images asset as11-40-5874 -f json
webcmd nasa-images metadata as11-40-5874 -f json
webcmd nasa-images captions 172_ISS-Slosh -f json
```

## Development

```bash
# Install locally for development (symlinked, changes reflect immediately)
webcmd plugin install file:///Users/rishabh/Developer/clis/webcmd-plugin-nasa-images

# Verify commands are registered
webcmd list | grep nasa-images

webcmd nasa-images search "apollo 11" --limit 3 -f json
webcmd nasa-images asset as11-40-5874 -f json
webcmd nasa-images metadata as11-40-5874 -f json
webcmd nasa-images captions 172_ISS-Slosh -f json
```
