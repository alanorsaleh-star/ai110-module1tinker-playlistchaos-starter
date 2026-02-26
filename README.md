Playlist Chaos: Week 1 Tinker Activity
This activity emphasized AI‑supported debugging and understanding how data flows between the Streamlit UI and the backend logic. I focused on the classification and statistics functions, which are likely the most confusing areas for students due to overlapping thresholds and keyword‑based matching. AI was helpful for clarifying complex expressions but occasionally suggested changes that conflicted with the app’s configuration. To guide a student without revealing the solution, I would have them print the song dictionary using st.write() to observe the exact inputs to the classification function.

Key Issues Identified:
  1. Artist searches returned no results
  2. Average energy was calculated only from Hype songs
  3. Hype ratio produced incorrect or unstable values

Fixes Applied:
  1. Reversed the search condition to correctly match queries within artist names
  2. Calculated average energy using all songs
  3. Corrected the Hype ratio denominator to use the full library size
  
Code Structure:
  1. app.py: Streamlit interface and user interactions
  2. playlist_logic.py: Normalization, classification, and statistical logic
  
Effective Strategies:
  1. Ask AI to explain logic rather than fix code
  2. Refresh the app after each change
  3. Use st.write() to inspect session state and verify data flow
