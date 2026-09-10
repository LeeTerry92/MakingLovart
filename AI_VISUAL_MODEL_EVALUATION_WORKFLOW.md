# AI Visual Model Evaluation Workflow

An infinite canvas is a useful place to compare image and video models because every result can remain visible beside its prompt, reference asset, and generation settings. The comparison becomes less reliable, however, when prompts or inputs change between runs.

This workflow keeps model evaluation controlled and makes the results reusable for later creative projects.

## 1. Define the production task

Start with a specific job instead of asking which model is "best." Examples:

- preserve a character while changing the background;
- render readable product packaging;
- convert a storyboard frame into a short camera move;
- create several views of the same object;
- extend an existing composition without changing the subject;
- generate a social clip in a fixed aspect ratio.

The winning model should be the one that handles the production constraint, not the one that produces the most dramatic isolated result.

## 2. Create a locked test cell

Place these items together on the canvas:

- the original prompt;
- negative constraints;
- reference images;
- aspect ratio and resolution;
- duration for video tests;
- model and version;
- date of the test;
- output images or clips.

Duplicate the full cell for every model. Change only the model selection during the first comparison round.

## 3. Separate prompt responsibilities

Use a prompt structure that can be inspected and revised:

1. **Preserve:** details that must remain unchanged.
2. **Subject:** the main person, object, or scene.
3. **Action:** one primary subject action.
4. **Camera:** framing or one camera movement.
5. **Environment:** lighting, weather, and secondary motion.
6. **Exclude:** defects or changes that would invalidate the result.

Do not combine several camera moves in the baseline test. Complex instructions can be added after the model demonstrates control over the simple case.

## 4. Evaluate images by dimension

Score each output separately:

| Dimension | Example checks |
| --- | --- |
| Prompt adherence | Required subject, action, composition, and exclusions |
| Identity | Face, hair, body proportions, clothing, and accessories |
| Geometry | Product shape, hands, object boundaries, and perspective |
| Typography | Spelling, legibility, placement, and style |
| Local editing | Whether unselected regions remain unchanged |
| Style consistency | Palette, rendering method, lighting, and texture |

Use a 1-5 scale and record a short failure note. A beautiful result with incorrect text or changed product geometry is not production-ready.

## 5. Evaluate videos by dimension

For image-to-video and text-to-video tests, add:

- first-frame fidelity;
- subject identity through the full clip;
- camera-path adherence;
- object geometry during motion;
- background stability;
- temporal flicker;
- final-frame usability;
- audio timing when generated audio is included.

Repeat each important prompt more than once. The best selected clip does not reveal repeatability. For controlled video comparisons, a [multi-model text-to-video workspace](https://photoartify.com/en/video-generator/text-to-video) can help run the same creative brief against different model families.

Disclosure: this external testing workspace is maintained by the PhotoArtify Team.

## 6. Calculate effective cost

Published credit prices are not enough. Track:

- generations attempted;
- outputs accepted;
- average queue time;
- manual correction time;
- export restrictions;
- watermark or resolution limits;
- credits consumed per accepted output.

A model with a higher per-generation price may be cheaper when it requires fewer retries.

## 7. Promote the winner to a reusable preset

After choosing a model, save a preset containing:

- provider and model version;
- prompt structure;
- reference requirements;
- preferred aspect ratio and resolution;
- negative constraints;
- known failure cases;
- acceptance thresholds.

Do not overwrite the original evaluation cells. Keep them as a visual record so future model updates can be tested against the same baseline.

## 8. Re-test after model updates

Model behavior can change without a workflow change. Re-run the baseline when:

- the provider announces a new version;
- prompt adherence changes unexpectedly;
- generation latency shifts materially;
- an old preset starts producing more failures;
- pricing or export limits change.

A stable evaluation canvas turns model selection from preference into a reproducible engineering decision.
