# Test plan

The browser test panel executes:
1. SceneGraph schema validation.
2. 2.5D Canvas PNG generation.
3. 2.5D PNG decode and dimensions.
4. WebGL context availability.
5. Three.js geometry creation.
6. 2.5D and 3D selection synchronization.
7. Import, undo and redo snapshot validation.
8. JSON serialization roundtrip.

Manual verification:
- Select a building in the object list and verify red highlight in 2.5D.
- Select a mesh in Three.js and verify the same object ID becomes selected.
- Create a history test edit; verify Undo and Redo counters and model position.
- Download the JSON test report and check passed, total, schemaErrors and history.
