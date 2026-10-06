# Complete feature inventory

## Input and analysis
- Upload PNG, JPG and WebP plans.
- Browser-side Canvas sampling specification for green ratio, dark structure ratio and edge density.
- SceneGraph JSON structure for grounds, buildings, trees, hedges and courtyard panels.

## 2.5D
- Procedural isometric coordinate conversion.
- Independent vertical faces and top faces.
- Selection highlight.
- PNG output and decode smoke tests.

## Three.js
- Multi-object buildings, grounds, trees and hedges.
- Raycaster object selection.
- Selection synchronization with 2.5D.
- WebGL availability and geometry tests.
- Resource disposal strategy.

## Editing and validation
- Object IDs and schema validation.
- Undo and redo transaction design.
- JSON serialization roundtrip.
- Downloadable test report.

## Integration specification
- Provider routing and fallback design.
- Job create, polling, cancellation and provider health contracts.
- Server-only secret list.
