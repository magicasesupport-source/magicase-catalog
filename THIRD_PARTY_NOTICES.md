# Catalog provenance and third-party rights

Card metadata and reference-image source: [Scryfall](https://scryfall.com/docs/api).
Reference images are used transiently to prepare features and are not bundled
in the distributed catalog packages. Card artwork, names, text and trademarks
remain subject to their respective owners' rights, including Wizards of the Coast.
Metadata identifiers and facts are not claimed as exclusive MagiCase property.

Feature extraction uses the DINOv2-S/14 model from Meta Platforms, Inc. and
affiliates, whose [base weights are identified as Apache-2.0](https://huggingface.co/facebook/dinov2-small/tree/ed25f3a31f01632728cabb09d1542f84ab7b0056).
The quantized ONNX conversion is identified by its publisher as a conversion of
those base weights:
[onnx-community/dinov2-small](https://huggingface.co/onnx-community/dinov2-small/tree/8b1f705a3a7f6f062f6bdd21986c1583d3ef105d).
Its model file SHA-256 is
`c179f8f7f592449c4c1bca4cd124a7538021428c5ffb89afde9503935b197efb`.
The converter repository does not add a separate explicit license tag; the
identified Apache-licensed base and conversion provenance are retained here.

No model weights, training datasets, OpenCV binaries or ONNX Runtime binaries are
distributed in these data packages. Their separate licenses are not replaced
or restricted by the MagiCase catalog license. License copies accompany those
components where the components themselves are distributed in the application.

The catalog format currently uses 384-byte signed-int8 signatures, normalized
RGB whole-card inputs and cosine similarity. These are prepared independently
for MagiCase and do not use CollectorVision, Milo or their precomputed embeddings.
This is reference generation with an existing model, not training a new model.

The limited-use license applies only where MagiCase holds applicable rights.
It does not create copyright in facts or machine-generated outputs, establish
that a particular database satisfies legal protection requirements, or remove
statutory exceptions or permissions granted by third-party licenses.
