# Scheduling games for the new Champions League format with Mixed Integer Programming

_Disclaimer: This project is for recreational purposes only. The software is provided under the MIT license._

Starting in September 2024, the UEFA Champions League will adopt a new format, transitioning from a group stage with 8 groups of 4 teams (32 teams total) to a league format with 36 teams. 
Detailed information about this new format can be found [here](https://www.uefa.com/uefachampionsleague/news/0268-12157d69ce2d-9f011c70f6fa-1000--new-format-for-champions-league-post-2024-everything-you-ne/).

Key Constraints:

- **Match Days**: 8 total match days
- **Games per Match Day**: Each of the 36 teams plays 1 game per match day
- **Home and Away Games**: Each team plays 4 games at home and 4 games away
- **Tier Division**: The 36 teams are divided into 4 tiers based on UEFA rankings
- **Tier Matches**: Each team plays against 2 teams from each tier (including their own tier)
- **No Country Derbies**: Teams will not play against others from the same federation
  
This project aims to create a feasible schedule by formulating an optimization model that includes binary decision variables, multiple linear constraints and no objective function. 
This is a classic case of Mixed Integer Programming. The solution generated will satisfy the constraints mentioned above.

The official schedule by UEFA will differ and likely incorporate additional constraints, such as:

1. **City Teams**: Teams from the same city (e.g., Inter Milan and AC Milan) will likely alternate their home and away games as much as possible to avoid playing at home on the same day.
2. **Broadcasting Considerations**: Potential adjustments for TV broadcasting requirements.
3. Other unknowns.

_Notice that the data used for the teams is partially accurate with the qualified teams up to late July 2024. The exact list will only be available in September after the playoff rounds will be completed! 
The list chosen in the notebook for the non qualified teams is purely random!_
