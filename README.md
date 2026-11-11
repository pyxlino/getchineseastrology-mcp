# Get Chinese Astrology MCP app

Calculate Chinese astrology charts from a birth date.

Ask for your BaZi Four Pillars, your zodiac year, how two animals match, your five elements, a Kua number, an I Ching reading, a Zi Wei Dou Shu chart or the Flying Stars of a year. The app uses the same calculations as getchineseastrology.com and draws the result.

- Website: https://getchineseastrology.com
- Documentation: https://getchineseastrology.com/app
- Privacy: https://getchineseastrology.com/privacy
- Terms: https://getchineseastrology.com/terms

This repository documents the hosted connector. It does not contain the
website or its code.

## Connect

- Endpoint: `https://getchineseastrology.com/api/mcp`
- Transport: Streamable HTTP
- Authentication: none (no account, sign-in or API key)

```json
{ "mcpServers": { "get-chinese-astrology": { "url": "https://getchineseastrology.com/api/mcp" } } }
```

In ChatGPT, add it as a custom MCP server with no authentication. In
Claude, open Customize, then Connectors, choose Add custom connector and enter the URL.

## Tools

All tools are read-only.

| Tool | What it does |
|---|---|
| `get_bazi_chart` | Calculates the Four Pillars (BaZi) chart for a birth date, an optional birth time and the birthplace time zone. |
| `get_zodiac_year` | Returns the Chinese zodiac year for a birth date or a calendar year: the animal, Heavenly Stem, element, yin or yang, the Chinese New Year dates that open and close the year and the Li Chun date. |
| `check_animal_compatibility` | Compares two Chinese zodiac animals, or the animals of two birth years, and names their relationship: Six Harmony, Three Harmony, clash, harm, break, punishment or neutral. |
| `count_five_elements` | Counts Wood, Fire, Earth, Metal and Water across the visible characters of the Four Pillars chart for a birth date, with an optional birth time and UTC offset. |
| `get_kua_number` | Returns the feng shui Kua number for a birth date and calculation table: its trigram, element, East or West group, and the four favourable and four unfavourable directions. |
| `cast_i_ching` | Reads an I Ching hexagram from six line values, bottom line first: 6 is a changing Yin line, 7 a Yang line, 8 a Yin line and 9 a changing Yang line. |
| `get_zi_wei_chart` | Builds a Zi Wei Dou Shu chart for a birth date, a birth time and a traditional calculation table. |
| `get_flying_stars` | Returns the annual Flying Stars chart for a year: the star in each of the nine palaces, the centre star and the moment Li Chun begins the year. |

## Try asking

- "What is my BaZi chart? I was born on 15 June 1990 at 12:30 in Shanghai."
- "Are the Rat and the Horse compatible?"
- "Show the Flying Stars chart for 2027."

## Report an issue

Open an issue in this repository or email support@getchineseastrology.com.

## License

The documentation files in this repository are MIT licensed (see
[LICENSE](LICENSE)). The Get Chinese Astrology website, its content, data and brand are
not covered by this license.
