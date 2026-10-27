# Same place or not

A judgment task for 4.580 Inquiry into Computation and Design, MIT.

Twenty pairs of street-level photographs. For each pair a participant decides
whether the two pictures show the same place, rates their confidence, and marks
on both images whatever settled the decision, labelled by category: building,
street furniture and signs, vegetation, ground, sky and skyline, people and
vehicles.

The study compares which streetscape elements people rely on against which ones
a visual place recognition model relies on, in order to ask which elements serve
both.

## The stimuli

Pairs are drawn from retrieval failures, so the hard negatives are images a
place recognition model actually ranked first rather than images picked by hand.
Ground truth comes from the camera positions recorded with the photographs.

| class | n | source |
|---|---|---|
| Same place, similar conditions | 5 | query against its ground truth |
| Same place, changed conditions | 5 | query against its ground truth, across weather or time of day |
| Different places, similar appearance | 5 | query against the image the model wrongly ranked first |
| Different places, obvious | 5 | across cities |

Photographs come from Mapillary Street-Level Sequences (Copenhagen, San
Francisco) and Tokyo 24/7, both public research datasets, and are reproduced
here only as stimuli for this coursework study.

## Answers

Responses are kept in the browser and exported as a JSON file at the end. No
server, no tracking, nothing leaves the participant's machine unless they send
the file.
