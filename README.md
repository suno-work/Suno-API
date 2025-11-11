# Suno-API
Suno API delivers advanced AI music capabilities through easy-to-integrate APIs, including music generation, lyrics creation, audio processing, and video production. Our platform is designed for developers and businesses who need:
-  99.9% Uptime - Reliable and stable API performance
-  Affordable Pricing - Transparent, usage-based pricing system
-  20-Second Streaming Output - Fast delivery with streaming response
-  High Concurrency - Scalable solutions that grow with your needs
-  24/7 Support - Professional technical assistance
-  Watermark-Free - Commercial-ready music generation
# Support & Community
-  24/7 Support - Contact our technical team anytime
-  Email Support - support@suno.work
-  Documentation Updates - Regular improvements and new features
-  API Status - Monitor real-time service status
-  Developer Resources - Comprehensive guides and best practices
# API Base URL
All API requests should be sent to: https://api.suno.work
# Authentication
All API requests require authentication using a Bearer token:

- Authorization: Bearer YOUR_API_KEY
 Obtain your API key from the Email Support : support@suno.work

# Price
Generate Music :$0.04 USD per call

# API DOCS

# Generate Music
post /api/generate/v2-web/
```json
{
	// "callBackUrl":"xxxxx",
  "generation_type": "TEXT",
  "title": "An Impossible Dream",
  "tags": "pop",
  "mv": "chirp-auk-turbo",//chirp-v2-xxl-alpha  chirp-v3-0  chirp-v3-5 chirp-v4 chirp-auk-turbo chirp-auk chirp-bluejay chirp-crow
  "prompt": "(Ooh-ooh…)\n\n[Verse 1] \nI chase a star beyond the sky  \nA wish too bold to ever try  \nThe world says stop, it can’t be done  \nYet in my heart, the race is won  \nYour voice echoes in empty halls  \nA promise no one else recalls  \n\n[Pre-Chorus]  \nThey laugh and say it’s all in vain  \nBut dreams don’t break in pouring rain  ",
  "make_instrumental": false
  
  
}
return
```json
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": [
        508874,
        508875
    ]
}
# Check Task Status
get /api/feed/v2/508874
return
```json
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "[{\"status\":\"complete\",\"title\":\"An Impossible Dream\",\"play_count\":0,\"upvote_count\":0,\"allow_comments\":true,\"id\":\"e6c83884-b4a7-448b-8f26-2911908e15d6\",\"entity_type\":\"song_schema\",\"video_url\":\"\",\"audio_url\":\"https://cdn1.suno.ai/e6c83884-b4a7-448b-8f26-2911908e15d6.mp3\",\"image_url\":\"https://cdn2.suno.ai/image_e6c83884-b4a7-448b-8f26-2911908e15d6.jpeg\",\"image_large_url\":\"https://cdn2.suno.ai/image_large_e6c83884-b4a7-448b-8f26-2911908e15d6.jpeg\",\"major_model_version\":\"v4.5-all\",\"model_name\":\"chirp-auk\",\"metadata\":{\"tags\":\"pop\",\"prompt\":\"(Ooh-ooh…)\\n\\n[Verse 1] \\nI chase a star beyond the sky  \\nA wish too bold to ever try  \\nThe world says stop, it can’t be done  \\nYet in my heart, the race is won  \\nYour voice echoes in empty halls  \\nA promise no one else recalls  \\n\\n[Pre-Chorus]  \\nThey laugh and say it’s all in vain  \\nBut dreams don’t break in pouring rain  \",\"type\":\"gen\",\"duration\":88.4,\"refund_credits\":false,\"stream\":true,\"can_remix\":true,\"is_remix\":false,\"priority\":0,\"has_stem\":false,\"uses_latest_model\":false,\"model_badges\":{\"songrow\":{\"display_name\":\"v4.5-all\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}}},\"is_liked\":false,\"user_id\":\"63613741-fa68-4947-925f-3497507bef95\",\"display_name\":\"5u41svhr\",\"handle\":\"5u41svhr\",\"is_handle_updated\":false,\"avatar_image_url\":\"https://cdn1.suno.ai/sAura1.jpg\",\"is_trashed\":false,\"created_at\":\"2025-11-11T02:01:07.607Z\",\"is_public\":false,\"explicit\":false,\"comment_count\":0,\"flag_count\":0,\"is_contest_clip\":false,\"has_hook\":false,\"batch_index\":0},{\"status\":\"complete\",\"title\":\"An Impossible Dream\",\"play_count\":0,\"upvote_count\":0,\"allow_comments\":true,\"id\":\"439e7659-85bd-4a18-a176-e73ad73a1da5\",\"entity_type\":\"song_schema\",\"video_url\":\"\",\"audio_url\":\"https://cdn1.suno.ai/439e7659-85bd-4a18-a176-e73ad73a1da5.mp3\",\"image_url\":\"https://cdn2.suno.ai/image_439e7659-85bd-4a18-a176-e73ad73a1da5.jpeg\",\"image_large_url\":\"https://cdn2.suno.ai/image_large_439e7659-85bd-4a18-a176-e73ad73a1da5.jpeg\",\"major_model_version\":\"v4.5-all\",\"model_name\":\"chirp-auk\",\"metadata\":{\"tags\":\"pop\",\"prompt\":\"(Ooh-ooh…)\\n\\n[Verse 1] \\nI chase a star beyond the sky  \\nA wish too bold to ever try  \\nThe world says stop, it can’t be done  \\nYet in my heart, the race is won  \\nYour voice echoes in empty halls  \\nA promise no one else recalls  \\n\\n[Pre-Chorus]  \\nThey laugh and say it’s all in vain  \\nBut dreams don’t break in pouring rain  \",\"type\":\"gen\",\"duration\":83.88,\"refund_credits\":false,\"stream\":true,\"can_remix\":true,\"is_remix\":false,\"priority\":0,\"has_stem\":false,\"uses_latest_model\":false,\"model_badges\":{\"songrow\":{\"display_name\":\"v4.5-all\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}}},\"is_liked\":false,\"user_id\":\"63613741-fa68-4947-925f-3497507bef95\",\"display_name\":\"5u41svhr\",\"handle\":\"5u41svhr\",\"is_handle_updated\":false,\"avatar_image_url\":\"https://cdn1.suno.ai/sAura1.jpg\",\"is_trashed\":false,\"created_at\":\"2025-11-11T02:01:07.607Z\",\"is_public\":false,\"explicit\":false,\"comment_count\":0,\"flag_count\":0,\"is_contest_clip\":false,\"has_hook\":false,\"batch_index\":1}]"
}

# Create Music Video
post /api/video/generate/
{
    // "callBackUrl":"xxxxx",
	"suno_id": "e6c83884-b4a7-448b-8f26-2911908e15d6"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508876
}
# Check Task Status
get /api/feed/v2/508876
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "{\"status\":\"complete\",\"video_url\":\"https://cdn1.suno.ai/e6c83884-b4a7-448b-8f26-2911908e15d6.mp4\"}"
}

# gen midi
post /api/gen/midi
{"suno_id":"e6c83884-b4a7-448b-8f26-2911908e15d6"}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508877
}


# lyrics infill
post /api/generate/lyrics-infill/
{
  "prompt": "dog",
  "context_lyrics_prefix": "I chase ",
  "context_lyrics_edit": "a star ",
  "context_lyrics_suffix": "beyond the sky ",
  "title": ""
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508878
}
# Check Task Status
get /api/feed/v2/508878
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "{\"lyrics_request_id\":\"edff8385-c336-4c72-ae18-8fc57017c2c1\",\"lyrics_id\":\"3f8d13e7-3e0b-495d-93f6-98f6da73d6a6\",\"generated_lyrics\":\"a bone \"}"
}

# upsample tags
post /api/generate/upsample-tags
{"original_tags":"pop"}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508879
}
# Check Task Status
get /api/feed/v2/508879
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "{\"upsampled_tags\":\"A pop track opens with catchy synth stabs and a tight, punchy drum groove. Verses feature clean guitar accents and warm bass underpinning airy layers. The pre-chorus adds vocal harmonies and subtle pads, then the chorus bursts with bright hooks, energetic beats, and dynamic production.\",\"request_id\":\"7b965b28-55f1-4ed5-bca7-98f1aa73bd77\"}"
}

# adjust speed
post /api/clips/adjust-speed/
{
    // "callBackUrl":"xxx",
  "clip_id": "e6c83884-b4a7-448b-8f26-2911908e15d6",
  "speed_multiplier": 2,
  "keep_pitch": true,
  "title": "An Impossible Dream (2x)"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508880
}
# Check Task Status
get /api/feed/v2/508880
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "[{\"status\":\"complete\",\"title\":\"An Impossible Dream (2x)\",\"play_count\":0,\"upvote_count\":0,\"allow_comments\":true,\"id\":\"ca78a9b1-5528-4651-a1d4-4da78d69d9c8\",\"entity_type\":\"song_schema\",\"video_url\":\"\",\"audio_url\":\"https://cdn1.suno.ai/ca78a9b1-5528-4651-a1d4-4da78d69d9c8.mp3\",\"image_url\":\"https://cdn2.suno.ai/image_e6c83884-b4a7-448b-8f26-2911908e15d6.jpeg\",\"image_large_url\":\"https://cdn2.suno.ai/image_large_e6c83884-b4a7-448b-8f26-2911908e15d6.jpeg\",\"major_model_version\":\"v4.5-all\",\"model_name\":\"chirp-auk\",\"metadata\":{\"tags\":\"pop\",\"prompt\":\"(Ooh-ooh…)\\n\\n[Verse 1] \\nI chase a star beyond the sky  \\nA wish too bold to ever try  \\nThe world says stop, it can’t be done  \\nYet in my heart, the race is won  \\nYour voice echoes in empty halls  \\nA promise no one else recalls  \\n\\n[Pre-Chorus]  \\nThey laugh and say it’s all in vain  \\nBut dreams don’t break in pouring rain  \",\"type\":\"edit_speed\",\"duration\":44.2,\"has_vocal\":false,\"can_publish_with_vocal\":false,\"speed_clip_id\":\"e6c83884-b4a7-448b-8f26-2911908e15d6\",\"can_remix\":true,\"is_remix\":true,\"has_stem\":false,\"uses_latest_model\":false,\"model_badges\":{\"songrow\":{\"display_name\":\"v4.5-all\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}}},\"is_liked\":false,\"user_id\":\"63613741-fa68-4947-925f-3497507bef95\",\"display_name\":\"5u41svhr\",\"handle\":\"5u41svhr\",\"is_handle_updated\":false,\"avatar_image_url\":\"https://cdn1.suno.ai/sAura1.jpg\",\"is_trashed\":false,\"created_at\":\"2025-11-11T02:22:48.576Z\",\"is_public\":false,\"is_following_creator\":false,\"comment_count\":0,\"flag_count\":0,\"is_contest_clip\":false,\"has_hook\":false,\"batch_index\":0}]"
}

# crop
post /api/edit/crop/
{
    // "callBackUrl":"xxx",
    "clip_id":"e6c83884-b4a7-448b-8f26-2911908e15d6",
    "crop_start_s":3,
    "crop_end_s":30,
    "is_crop_remove":false
}

# billing
get /api/billing/info/
return
{
    "data": "99.00000",
    "code": 200,
    "error": "",
    "status": 3
}

# generate lyrics pair
post /api/generate/lyrics-pair
{
	// "callBackUrl":"xxx",
	"prompt":"An Impossible Dream",
	"lyricsModel": "remi-v1"//  default  or remi-v1
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508882
}
# Check Task Status
get /api/feed/v2/508882
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "{\"ret_a\":{\"title\":\"An Impossible Dream\",\"text\":\"[Verse]\\nI reached for the sky with my bare hands\\nA fool's grip on the edge of the clouds\\nThe stars whispered secrets I couldn’t understand\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Verse 2]\\nI built a ladder from shattered hope\\nClimbing high where the air is thin\\nEach rung a promise\\nEach promise a rope\\n\\n[Prechorus]\\nThe higher I go\\nThe farther it seems\\nIs it the end or just more dreams\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Bridge]\\nIs it madness or magic\\nThis chase I adore\\nA horizon that runs when I reach for more\\nBut what is life without the fight\\nWithout the climb\\nWithout the flight\",\"status\":\"complete\",\"errorMsg\":\"\",\"tags\":[\"cinematic\",\"emotional; sweeping strings and a haunting piano melody build with dynamic crescendos and soft descents\",\"orchestral\"]},\"ret_b\":{\"title\":\"An Impossible Dream\",\"text\":\"[Verse]\\nI reached for the moon with paper wings\\nFell through the sky where silence sings\\nEvery star laughed as I passed by\\nThey whispered\\n“you’ll never learn to fly”\\n\\n[Prechorus]\\nBut what if I could\\nWhat if I might\\nTurn this darkness into light\\n\\n[Chorus]\\nAn impossible dream\\nThat’s what they said\\nChasing the clouds\\nWhere angels tread\\nAn impossible dream\\nI’ll make it true\\nBecause impossible means nothing to you\\n\\n[Verse 2]\\nI built a ship from broken glass\\nSailed on rivers of my shattered past\\nEach crack reflected the world’s disdain\\nBut I held the helm through every pain\\n\\n[Prechorus]\\nAnd what if I fall\\nWhat if I break\\nEven mountains move with one small quake\\n\\n[Chorus]\\nAn impossible dream\\nThat’s what they said\\nChasing the clouds\\nWhere angels tread\\nAn impossible dream\\nI’ll make it true\\nBecause impossible means nothing to you\",\"status\":\"complete\",\"errorMsg\":\"\",\"tags\":[\"pop ballad\",\"piano-driven with lush string layers\",\"ethereal\"]}}"
}

# cover
post /api/generate/v2-web/
{
  "generation_type": "TEXT",
  "mv": "chirp-auk-turbo",
  "gpt_description_prompt": "",
  "prompt": "[Verse]\nI reached for the sky with my bare hands\nA fool's grip on the edge of the clouds\nThe stars whispered secrets I couldn’t understand\n\n[Chorus]\nAn impossible dream keeps calling my name\nLike fire in the rain\nIt burns just the same\nI chase it\nI break it\nIt’s always out of frame\nAn impossible dream\nOh it’s a beautiful game\n\n[Verse 2]\nI built a ladder from shattered hope\nClimbing high where the air is thin\nEach rung a promise\nEach promise a rope\n\n[Prechorus]\nThe higher I go\nThe farther it seems\nIs it the end or just more dreams\n\n[Chorus]\nAn impossible dream keeps calling my name\nLike fire in the rain\nIt burns just the same\nI chase it\nI break it\nIt’s always out of frame\nAn impossible dream\nOh it’s a beautiful game\n\n[Bridge]\nIs it madness or magic\nThis chase I adore\nA horizon that runs when I reach for more\nBut what is life without the fight\nWithout the climb\nWithout the flight",
  "title": "An Impossible Dream (extend)",
  "tags": "Funk",
  "metadata": {
    "vocal_gender": "m",
    "create_mode": "custom",
    "control_sliders": {
      "style_weight": 0.9,
      "weirdness_constraint": 0.1
    },
    "can_control_sliders": [
      "style_weight",
      "weirdness_constraint"
    ]
  },
  "task": "cover",
  "cover_clip_id": "4edc9d06-5a54-470a-8697-e6b82f7bf3cf"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": [
        508888,
        508889
    ]
}

# extend
post /api/generate/v2-web/
{
  "generation_type": "TEXT",
  "mv": "chirp-auk-turbo",
  "gpt_description_prompt": "",
  "prompt": "[Verse]\nI reached for the sky with my bare hands\nA fool's grip on the edge of the clouds\nThe stars whispered secrets I couldn’t understand\n\n[Chorus]\nAn impossible dream keeps calling my name\nLike fire in the rain\nIt burns just the same\nI chase it\nI break it\nIt’s always out of frame\nAn impossible dream\nOh it’s a beautiful game\n\n[Verse 2]\nI built a ladder from shattered hope\nClimbing high where the air is thin\nEach rung a promise\nEach promise a rope\n\n[Prechorus]\nThe higher I go\nThe farther it seems\nIs it the end or just more dreams\n\n[Chorus]\nAn impossible dream keeps calling my name\nLike fire in the rain\nIt burns just the same\nI chase it\nI break it\nIt’s always out of frame\nAn impossible dream\nOh it’s a beautiful game\n\n[Bridge]\nIs it madness or magic\nThis chase I adore\nA horizon that runs when I reach for more\nBut what is life without the fight\nWithout the climb\nWithout the flight",
  "title": "An Impossible Dream (extend)",
  "tags": "Funk",
  "metadata": {
    "vocal_gender": "m",
    "create_mode": "custom",
    "control_sliders": {
      "style_weight": 0.9,
      "weirdness_constraint": 0.1
    },
    "can_control_sliders": [
      "style_weight",
      "weirdness_constraint"
    ]
  },
  "task": "extend",
  "continue_at": 40,
  "continue_clip_id": "4edc9d06-5a54-470a-8697-e6b82f7bf3cf"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": [
        508883,
        508884
    ]
}
# Check Task Status
get /api/feed/v2/508883
return
{
    "error": null,
    "status": 3,
    "code": 200,
    "data": "[{\"status\":\"complete\",\"title\":\"An Impossible Dream (extend)\",\"play_count\":0,\"upvote_count\":0,\"allow_comments\":true,\"id\":\"97d522b4-35b1-4fee-90af-3eae6f3c355f\",\"entity_type\":\"song_schema\",\"video_url\":\"\",\"audio_url\":\"https://cdn1.suno.ai/97d522b4-35b1-4fee-90af-3eae6f3c355f.mp3\",\"image_url\":\"https://cdn2.suno.ai/image_97d522b4-35b1-4fee-90af-3eae6f3c355f.jpeg\",\"image_large_url\":\"https://cdn2.suno.ai/image_large_97d522b4-35b1-4fee-90af-3eae6f3c355f.jpeg\",\"major_model_version\":\"v4.5-all\",\"model_name\":\"chirp-auk\",\"metadata\":{\"tags\":\"Funk\",\"prompt\":\"[Verse]\\nI reached for the sky with my bare hands\\nA fool's grip on the edge of the clouds\\nThe stars whispered secrets I couldn’t understand\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Verse 2]\\nI built a ladder from shattered hope\\nClimbing high where the air is thin\\nEach rung a promise\\nEach promise a rope\\n\\n[Prechorus]\\nThe higher I go\\nThe farther it seems\\nIs it the end or just more dreams\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Bridge]\\nIs it madness or magic\\nThis chase I adore\\nA horizon that runs when I reach for more\\nBut what is life without the fight\\nWithout the climb\\nWithout the flight\",\"gpt_description_prompt\":\"\",\"history\":[{\"id\":\"4edc9d06-5a54-470a-8697-e6b82f7bf3cf\",\"continue_at\":40,\"type\":\"gen\",\"source\":\"web\",\"infill\":false}],\"edited_clip_id\":\"4edc9d06-5a54-470a-8697-e6b82f7bf3cf\",\"continue_at\":40,\"type\":\"gen\",\"duration\":174.28,\"refund_credits\":false,\"stream\":true,\"infill\":false,\"task\":\"extend\",\"can_remix\":true,\"is_remix\":false,\"priority\":0,\"has_stem\":false,\"uses_latest_model\":false,\"model_badges\":{\"songrow\":{\"display_name\":\"v4.5-all\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}},\"secondary_badges\":[{\"display_name\":\"Part 2\",\"icon_key\":\"part\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}]},\"is_liked\":false,\"user_id\":\"63613741-fa68-4947-925f-3497507bef95\",\"display_name\":\"5u41svhr\",\"handle\":\"5u41svhr\",\"is_handle_updated\":false,\"avatar_image_url\":\"https://cdn1.suno.ai/sAura1.jpg\",\"is_trashed\":false,\"created_at\":\"2025-11-11T02:37:57.750Z\",\"is_public\":false,\"explicit\":false,\"comment_count\":0,\"flag_count\":0,\"is_contest_clip\":false,\"has_hook\":false,\"batch_index\":0},{\"status\":\"complete\",\"title\":\"An Impossible Dream (extend)\",\"play_count\":0,\"upvote_count\":0,\"allow_comments\":true,\"id\":\"2fa7ebfb-e2ed-4a54-9d4c-c36ec8d260b7\",\"entity_type\":\"song_schema\",\"video_url\":\"\",\"audio_url\":\"https://cdn1.suno.ai/2fa7ebfb-e2ed-4a54-9d4c-c36ec8d260b7.mp3\",\"image_url\":\"https://cdn2.suno.ai/image_2fa7ebfb-e2ed-4a54-9d4c-c36ec8d260b7.jpeg\",\"image_large_url\":\"https://cdn2.suno.ai/image_large_2fa7ebfb-e2ed-4a54-9d4c-c36ec8d260b7.jpeg\",\"major_model_version\":\"v4.5-all\",\"model_name\":\"chirp-auk\",\"metadata\":{\"tags\":\"Funk\",\"prompt\":\"[Verse]\\nI reached for the sky with my bare hands\\nA fool's grip on the edge of the clouds\\nThe stars whispered secrets I couldn’t understand\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Verse 2]\\nI built a ladder from shattered hope\\nClimbing high where the air is thin\\nEach rung a promise\\nEach promise a rope\\n\\n[Prechorus]\\nThe higher I go\\nThe farther it seems\\nIs it the end or just more dreams\\n\\n[Chorus]\\nAn impossible dream keeps calling my name\\nLike fire in the rain\\nIt burns just the same\\nI chase it\\nI break it\\nIt’s always out of frame\\nAn impossible dream\\nOh it’s a beautiful game\\n\\n[Bridge]\\nIs it madness or magic\\nThis chase I adore\\nA horizon that runs when I reach for more\\nBut what is life without the fight\\nWithout the climb\\nWithout the flight\",\"gpt_description_prompt\":\"\",\"history\":[{\"id\":\"4edc9d06-5a54-470a-8697-e6b82f7bf3cf\",\"continue_at\":40,\"type\":\"gen\",\"source\":\"web\",\"infill\":false}],\"edited_clip_id\":\"4edc9d06-5a54-470a-8697-e6b82f7bf3cf\",\"continue_at\":40,\"type\":\"gen\",\"duration\":149.52,\"refund_credits\":false,\"stream\":true,\"infill\":false,\"task\":\"extend\",\"can_remix\":true,\"is_remix\":false,\"priority\":0,\"has_stem\":false,\"uses_latest_model\":false,\"model_badges\":{\"songrow\":{\"display_name\":\"v4.5-all\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}},\"secondary_badges\":[{\"display_name\":\"Part 2\",\"icon_key\":\"part\",\"light\":{\"text_color\":\"7D7C83\",\"background_color\":\"00000000\",\"border_color\":\"0000001A\"},\"dark\":{\"text_color\":\"A3A3A3\",\"background_color\":\"00000000\",\"border_color\":\"FFFFFF1A\"}}]},\"is_liked\":false,\"user_id\":\"63613741-fa68-4947-925f-3497507bef95\",\"display_name\":\"5u41svhr\",\"handle\":\"5u41svhr\",\"is_handle_updated\":false,\"avatar_image_url\":\"https://cdn1.suno.ai/sAura1.jpg\",\"is_trashed\":false,\"created_at\":\"2025-11-11T02:37:57.750Z\",\"is_public\":false,\"explicit\":false,\"comment_count\":0,\"flag_count\":0,\"is_contest_clip\":false,\"has_hook\":false,\"batch_index\":1}]"
}

# concat
post /api/generate/concat/v2/
{
    // "callBackUrl":"xxx",
    "clip_id":"97d522b4-35b1-4fee-90af-3eae6f3c355f"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508885
}

# persona
post /api/persona/create/
{
    // "callBackUrl":"xxx",
	"root_clip_id": "97d522b4-35b1-4fee-90af-3eae6f3c355f",
	"name": "An Impossible Dream",
	"description": "",
	"image_s3_id": null,
	"clips": [
	"97d522b4-35b1-4fee-90af-3eae6f3c355f"
	],
	"is_public": true
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508887
}

# uploads
post /api/uploads/audio/
{
	"url":"https://cdn1.suno.ai/97d522b4-35b1-4fee-90af-3eae6f3c355f.mp3",
	"type":"upload"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508890
}

# convert wav
post /api/gen/convert_wav/
{
    "suno_id":"97d522b4-35b1-4fee-90af-3eae6f3c355f"
}
return
{
    "error": "",
    "status": 3,
    "code": 200,
    "data": 508890
}
