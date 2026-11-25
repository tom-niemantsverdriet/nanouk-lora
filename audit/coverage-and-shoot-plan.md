# LoRA photo audit and shoot plan

Book **one 65–75 minute visit** for close portraits and waist-up lifestyle images. Aim for **30 selected photos from distinct captures**, with 16 core training candidates, eight held-out references, and six training backups. Use two training setups and two separate reference setups at the same location. The archive already supplies plenty of fitness, swimwear, and full-body poses. The priority is recognizable facial likeness in everyday lighting, with clear evidence for both sides of the face and her natural smiles.

## Archive coverage

The [populated scorecard](photo-audit.csv) covers all 99 source files. It identifies three exact duplicate copies and 28 additional files grouped provisionally with similar captures. That leaves **68 provisional capture groups**, including one on human-review hold. The grouping is conservative and can be refined if capture history establishes independent evidence. Among the files, 63 scored **2** for usable source quality on first review, 35 scored **1** for a documented compromise, and one scored **0** while review is pending. Of the 67 provisional representatives that were rated, 13 had clear facial cues, 20 were marginal, and 34 offered no usable face evidence in this screen. The shortlist contains 14 face candidates and 22 context candidates. These categories guide review order.

| What the archive has | Where it helps | Limitation |
| --- | --- | --- |
| Readable close portraits and selfies in car, cabin, covered daylight, and indoor lighting | General likeness, smile, styling, and lighting variation. Start with [IMG_1098.JPG](../source/IMG_1098.JPG), [IMG_1941.JPG](../source/IMG_1941.JPG), and [IMG_1865.JPG](../source/IMG_1865.JPG). | Many are near-frontal, tilted, smiling, pursed, or lit strongly from one side. The neutral eye-level anchor still needs a clean match. |
| Two close relatives of a waist-up teeth-smile photo | [IMG_1785.JPG](../source/IMG_1785.JPG) is the preferred lead. [IMG_1784.JPG](../source/IMG_1784.JPG) is its grouped alternate. | Both use the same elevated reclining fitness setup. Side, near-face hand, and lifestyle fit need checking. Count at most one group. |
| 51 beach-sunset files provisionally grouped into 35 captures within one apparent editorial session | Swimwear, light, standing and reclining poses, and some wider faces. [IMG_2209.JPG](../source/IMG_2209.JPG) and [IMG_2223.JPG](../source/IMG_2223.JPG) group together. [IMG_2253.JPG](../source/IMG_2253.JPG) adds direct-light face context. | Surroundings and styling recur, and many faces are small. Keep beach selects sparse in a general-purpose pilot. |
| Indoor full-body, gym, and mirror photos | Position, silhouette, and clothing variety. [IMG_1542.JPG](../source/IMG_1542.JPG) and [IMG_1614.JPG](../source/IMG_1614.JPG) are context leads. | Phone overlap, distance, or cropping limits identity evidence. |

The ratings use the [research rubric](../research/flux-lora-dataset-research.md#dataset-readiness). Thirty files were inspected using local 768-pixel short-edge previews, 68 used contact sheets, and [IMG_4387.JPG](../source/IMG_4387.JPG) stayed text-only pending a creator or human check on clothing coverage. Preview face measurements are approximate and live in separate columns. The installed FluxGym configuration, final buckets, and training crops were unavailable, so the scorecard leaves actual bucket measurements and confirmed scenario credit open. Session IDs use local capture-day metadata and visible context as working proxies. The beach sequence has one provisional session ID and three apparent styling setups. Confirm uncertain session or mirror information before counting coverage.

## Facial combinations to fill

The close portrait and waist-up lifestyle briefs below are provisional. Settle which looks will actually be posted before the visit. Left and right mean **her** left and right, using the cheek with more visible surface as the reference. Confirm it with the photographer in person and capture unmirrored originals.

| Scenario | Archive finding | Core training target | Held-out reference target |
| --- | --- | --- | --- |
| **R1 · weight 3** · Straight-on, neutral close portrait, eye-level, soft light | [IMG_1865.JPG](../source/IMG_1865.JPG) has directional cabin light and pursed lips. [IMG_2311.JPG](../source/IMG_2311.JPG) has a smile and a glass close to the face. No strong match surfaced. | 4, two in each training setup | 2, one in each reference setup |
| **R2 · weight 2** · Left three-quarter close portrait, relaxed smile | [IMG_1503.JPG](../source/IMG_1503.JPG) offers a relaxed expression, with a near-frontal head turn and red lighting. No strong left-side match surfaced. | 4, two in each training setup | 2, one in each reference setup |
| **R3 · weight 3** · Right three-quarter waist-up, teeth smile | One plausible archive group around [IMG_1785.JPG](../source/IMG_1785.JPG), with side, hand, and setting caveats. No independent second setup surfaced. | 4, two in each training setup | 2, one in each reference setup |
| **R4 · weight 2** · Left three-quarter waist-up, relaxed smile | [IMG_5089.JPG](../source/IMG_5089.JPG) has a readable near-frontal face in a high camera angle. No strong left-side match surfaced. | 4, two in each training setup | 2, one in each reference setup |

Four distinct qualifying training captures over two setups would reach the report’s maximum coverage level for each scenario. The two-setup minimum can still survive the loss of an individual capture. The archive has **zero confirmed scenario counts** at this stage. An aggregate readiness score would depend on the selected split and the actual trainer crops. [Coverage thresholds](../research/flux-lora-dataset-research.md#priority-combinations-and-coverage-levels)

## One visit shot list

Work at one site with soft indoor light and a nearby open-shade or alternate indoor area. Bring two everyday looks and a simple removable layer. Start with familiar styling and keep hair clear of eyes, cheeks, and jaw for the core photos. Use a rear camera or photographer at a comfortable portrait distance, generally around eye level. Leave room for the intended vertical 4:5 post crop. For each planned capture, take a few frames as insurance against blinks or blur and pick one. The select counts below refer to distinct observations.

| Block | Setup and direction | Selects | Time |
| --- | --- | ---: | ---: |
| **A · Train** | Soft window light, plain background, outfit one. Repeat R1–R4 twice. For the close shots, vary gaze or camera position while retaining the same yaw and expression. For waist-up, use one standing and one seated pose. | 8 | 15 min |
| **B · Train** | Open shade or a different softly lit background, outfit two. Repeat all four scenarios and the two distinct takes per scenario. Preserve the required cheek and smile so each is seen with different light and wardrobe. | 8 | 15 min |
| **Backups · Train** | While A or B is set up, take six additional combinations listed below. These are the buffer if the first LoRA needs more range. | 6 | 8–10 min |
| **C · Holdout** | Use a third camera position and background and soft light. Capture each required scenario once using a layer or styling variation. Label the entire setup **holdout** at capture. | 4 | 8 min |
| **D · Holdout** | Use a fourth background and a different light direction or camera placement. Capture each required scenario once. Maintain comparable head angles and expressions so these work as independent likeness references. Label the entire setup **holdout**. | 4 | 8 min |
| **Review** | Check the files against the four scenarios, verify the split and confirm the keepers with the creator. Repeat any missing or compromised capture while the setup is still available. | — | 7–10 min plus transitions |

Capture the **six backups** in this order.

1. Close right three-quarter, relaxed smile.
2. Close right three-quarter, natural teeth smile.
3. Waist-up left three-quarter, natural teeth smile.
4. Waist-up right three-quarter, relaxed smile.
5. Close left three-quarter, neutral.
6. Close right three-quarter, neutral.

If head-to-toe fashion or true profile is a **required deliverable**, add its own train and holdout block to this visit. For full-body, plan at least four distinctly posed training selects across A and B plus one genuine reference in each of C and D. For profile, use the same allocation for each required side and framing. Budget roughly **10–15 extra minutes for one such block**, with a larger allowance if both sides or multiple post types are required. The existing beach and mirror images can support body poses as needed. The core appointment estimate assumes close portraits and waist-up lifestyle.

### Before the creator leaves

- Check off all 16 core and eight reference selects by scenario and setup. Confirm visible eyes and jaw, correct side, clean expression, and headroom. Make sure the teeth smile still looks like her and stays visible at the intended waist-up crop.
- Review one representative crop per scenario at display size and magnification. Fix any backlight, focus, tight cropping, hair or hand overlap, and mirrored exports on site. Capture a fresh take if two selected photos are effectively a burst of the same pose.
- Keep C and D in a separate holdout folder. Two setups on the same visit give varied reference conditions. A separate existing reference session can supplement them if a specific judgment remains ambiguous.

## First training set and retest

Build a first candidate set of about **20–24 training representatives**. Start with the 16 qualified core captures and add about four to eight archive or backup groups for independent looks and useful variation. Start archive review with the covered-daylight portrait, car portrait, cabin portrait, and one different face or context setup that matches the briefs. Use at most one representative per group. Save the remainder of the backups for a targeted swap. Keep all holdout images out of training and generation conditioning.

Verify effective FluxGym crops, permissions, captions, and mirror status before committing the split. Recompute readiness once each required scenario has checked training representatives and holdout references. Use the report’s fixed ComfyUI prompts and seeds to test facial likeness on the face crop and at post size. If a failure repeats after checkpoint, strength, caption, and crop checks, try a same-size swap using the relevant captured backup and compare it on the same grid. A passing confirmation run across the required briefs is the stop point. [Pilot and photo intervention protocol](../research/flux-lora-dataset-research.md#matched-pilot-and-evaluation)
