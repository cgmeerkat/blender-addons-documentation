CycleAcoustics Version History
******************************

1.2.1 - 16 Apr 2025
-------------------
User-friendly error message if user tries to generate an IR without having rendered.

1.2.0 - 11 Aug 2024
-------------------
Added an option to exclude direct sound from IR outputs in order to get "wet only" IRs for use in music production with dry/wet mixing. Patched a bug that makes polarity incorrect. Compositing change: made the alpha values of "empty" pixels 1 (from 0.5 in the previous version); this change makes no difference to audio output and just improves rendered images’ visual clarity to users.

1.1.0 - 6 Aug 2024
------------------
More accurate binaural processing. Calculation for direction-based time difference between left and right ears is more accurate. Improved high-frequency sound reproduction for reflections at fractional-sample delays by using sinc interpolation. The sound emitter material now correctly accounts for travel times from emitters to first bounces.

1.0.0 - 2 Aug 2024
------------------
Initial Release
