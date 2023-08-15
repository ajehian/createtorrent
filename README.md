# Description

createtorrent is basically a wrapper for mktorrent which simplifies the process of creating a torrent.

You set up your personal announce URL in the `announce_url.conf` file and basically you're done!

Gone are the days where you need to calculate the piece size of the torrent file or memorize all the mktorrent parameters.

### Default parameters used for mktorrent:

- `-p` private flag which is required in private trackers
- `-l <size>` torrent piece size which is derived from `torrent_piece_size.conf`
- `-s <SOURCE>` source flag which corresponds to `announce_url.conf`
- `-a <ANNOUNCE URL>` announce URL flag which corresponds to `announce_url.conf`
- `-o <OUTPUT DIR>` torrent output which defaults to `$HOME/torrents`

# Requirements

- Any usable Linux distribution
- **mktorrent >= 1.1**

# Installation

- Clone the repo
- Create a configuration file `announce_url.conf`, using the included example as a guide
- Make sure the file is executable: `chmod +x` `createtorrent`

# Usage

`$ createtorrent /home/user/MyEncode/ PTP`
