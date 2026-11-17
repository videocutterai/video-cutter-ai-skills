# Video Clip Planner by Video Cutter AI

Plan trims, highlight clips, and portrait reframing for long videos. Give your agent a transcript with timestamps, chapter markers, or scene notes. It will suggest a cut list and flag shots where a vertical crop might lose a speaker, slide, or key action.

## Install

```sh
npx skills add videocutterai/video-cutter-ai-skills --skill video-clip-planner
```

## Try it

- “Use Video Clip Planner to find three standalone highlights in this timestamped interview transcript. Give me the opening line and source time range for each clip.”
- “Plan a 9:16 cut of this landscape webinar. Keep the slides readable and flag shots where both speakers need to stay in frame.”

The skill produces an edit plan. If you want to process footage in a browser, open the suggested [Video Cutter AI](https://video-cutter.ai/) tool and choose the media to submit.

## Worked example with podcast subtitles

This fictional editing podcast excerpt includes source timecodes and camera notes. Paste the excerpt into your agent and ask Video Clip Planner for three standalone Shorts with a source range, opening line, and 9:16 framing for each.

```text
00:10–00:14 Host: Let's talk about making short clips from interviews.
00:14–00:22 Guest: The best clip rarely starts with the question. Start with the line that makes a stranger want the answer.
00:22–00:30 Guest: In our interview episode, that line was “Your first question is usually too broad.” Then we showed how to narrow it.
00:30–00:38 Guest: Instead of asking “How did you get started?”, ask “What did you do on day one?” Now the story has somewhere to go.

01:05–01:13 Guest: One short should make one promise. If your opening promises a faster edit, show the edit before you talk about captions.
01:13–01:21 Guest: I split one answer into two clips. The first showed where to cut. The second showed how to clean up the subtitles.
01:21–01:29 Guest: That gave both clips a clear ending. A viewer could watch either one without needing the rest of the episode.
01:29–01:34 Host: We'll link the episode in the show notes.

02:04–02:12 Guest: A vertical crop can hide the whole point. Here the slide says hook, example, payoff. The words are part of the lesson.
02:12–02:20 Guest: When I center the crop on my face, the example disappears. So I put the slide above me instead.
02:20–02:29 Guest: Before exporting, I check the preview on my phone. If the captions cover the slide, I move them or give the slide more room.
```

The first passage uses a guest close-up with hand gestures. The second uses a wide shot of both speakers. The third shows the guest beside a slide labeled “Hook → Example → Payoff.”

| Short | Source start → end | Opening line | 9:16 framing |
| --- | --- | --- | --- |
| Open on the answer | 00:14 → 00:38 (24 s) | “The best clip rarely starts with the question.” | Center the guest in a medium crop. Leave room for their hands and check that captions stay clear of the gestures. |
| Make one promise per short | 01:05 → 01:29 (24 s) | “One short should make one promise.” | Stack crops from the wide shot with the guest above the host. If either face would be too small, fit the wide shot inside the vertical frame with padding. |
| Keep slide text readable | 02:04 → 02:29 (25 s) | “A vertical crop can hide the whole point.” | Place the full slide above the guest. Keep captions in the speaker panel and check that all three slide labels are readable on a phone. |

Each selection opens with a complete idea and ends with a concrete example or takeaway. The host's setup and show-notes plug can stay out of the cuts.

[Read the skill](SKILL.md) · [MIT-0 license](LICENSE)
