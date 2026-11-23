# Freebeat for Claude

Turn a song into a music video, an animated lyric video or a dance video, right in the conversation. Freebeat's AI director plans the video, generates it and times it to the song. Bring your song as a public link to an audio file or a music page, or let Freebeat write an original song from your idea first. You can let the director run automatically or co-create with it: it shows its plan, the images and clips it made, and takes your notes.

Also create and edit images, turn text or images into short video clips, make a photo sing a track, lip-sync an existing clip to new audio, and turn a photo into a video with an effect template.

## How it works

This plugin connects Claude to Freebeat's hosted MCP server at `https://freebeat.ai/api/mcp` and adds skills that tell Claude which Freebeat tool fits each request. When you first use it, Claude asks you to sign in to your Freebeat account (OAuth); no API key is needed.

Generations use your existing Freebeat credits. Before a paid generation starts, Claude states the price, or says when the total cost can't be known in advance, and asks for your consent. Finished videos open on freebeat.ai, where you can also continue editing.

## Links

- Website and setup guide: https://freebeat.ai/mcp
- Privacy policy: https://freebeat.ai/privacy-policy
- Terms of service: https://freebeat.ai/terms-of-service
- Support: support@freebeat.ai, https://freebeat.ai/contact
