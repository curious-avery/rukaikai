# RuKaiKai source and data notices

RuKaiKai combines original application code with language resources from several
sources. Downloading the local starter kit does not erase or replace the rights
and conditions attached to those sources.

## RuKaiKai project material

The interface, retrieval logic, prompts, and source organization were created for
the RuKaiKai language-preservation project by Avery Liu and Theavy So. The
Paiwan–English word list and study-reference sentences were supplied to this
project and are included in the local kit at the project owner’s direction.
Anyone planning to republish or redistribute those datasets should first confirm
permission from the underlying rights holders.

RuKaiKai was developed in consultation with Paiwan chief 葛關復勇
(Ge,Kuan-Fu-Yung), a faculty member at National Kaohsiung University of Science
and Technology. This acknowledgment records consultation only; it does not
imply individual or institutional endorsement, certification, or community-wide
validation.

## Ferrell dictionary material

Raleigh Ferrell, *Paiwan Dictionary* (1982), Pacific Linguistics C-73,
Australian National University. The source is available through ANU at
<https://openresearch-repository.anu.edu.au/>.

Dictionary-derived structured material follows the CC BY-SA 4.0 notice associated
with the supplied online edition. RuKaiKai’s organization, transcription of the
reviewed addenda, and rule summaries are identified as project changes. Raw OCR
spellings are not used as runtime evidence because the scan’s text layer corrupts
the phonemic characters ḍ and ł.

CC BY-SA 4.0: <https://creativecommons.org/licenses/by-sa/4.0/>

## Models and local runtimes

The starter kit does not contain Ollama, Node.js, or model weights. Those are
downloaded from their official sources and retain their own licenses and terms.
The recommended `qwen3:4b-instruct` model is retrieved through Ollama’s official
model registry.

## Interface dependencies

Third-party JavaScript package names and versions are recorded in
`package-lock.json`. The bundled shadcn Tailwind stylesheet carries its original
license notice in `vendor/shadcn-tailwind-4.13.0.LICENSE.md`.
