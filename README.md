# Freebeat for Claude

Turn a song into a music video, an animated lyric video or a dance video, right in the conversation. Freebeat's AI director plans the video, generates it and times it to the song. Bring your song as a public link to an audio file or a music page, or let Freebeat write an original song from your idea first. You can let the director run automatically or co-create with it: it shows its plan, the images and clips it made, and takes your notes.

Also create and edit images, turn text or images into short video clips, make a photo sing a track, lip-sync an existing clip to new audio, and turn a photo into a video with an effect template.

## How it works

This plugin connects Claude to Freebeat's hosted MCP server at `https://freebeat.ai/api/mcp` and adds skills that tell Claude which Freebeat tool fits each request. When you first use it, Claude asks you to sign in to your Freebeat account (OAuth); no API key is needed.

Generations use your existing Freebeat credits. Before a paid generation starts, Claude states the price, or says when the total cost can't be known in advance, and asks for your consent. Finished videos open on freebeat.ai, where you can also continue editing.

## Data and where it goes

- The plugin's tools run on Freebeat's MCP server at `https://freebeat.ai/api/mcp`. Your prompts, the links you share (songs, photos, clips) and the results are stored in your Freebeat account, where you can see them on freebeat.ai. Freebeat sends the material a generation needs to the AI model providers it uses for that generation.
- In Claude Code, if you have the Freebeat CLI installed and signed in, some skills can use it to upload a local file (`freebeat --json assets upload-audio` / `upload-image`) or read a task result. The CLI sends that file or request to Freebeat's API at `https://api.freebeatfit.com`, the same service behind the MCP server.
- The plugin does not read your Claude chat history, memory or files beyond what you ask it to upload.

## Links

- Website and setup guide: https://freebeat.ai/mcp
- Privacy policy: https://freebeat.ai/privacy-policy
- Terms of service: https://freebeat.ai/terms-of-service
- Support: support@freebeat.ai, https://freebeat.ai/contact
