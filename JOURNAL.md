## Week 7 — Issue selection

**Issue link:** https://github.com/ascherj/pathreview/issues/37

**Issue title:** Add snapshot tests for prompt templates to catch accidental changes

**Tier:** [Yes] Tier 1  [ ] Tier 2  [ ] Tier 3

**Problem summary:**
Currently, LLM prompt templates can be silently changed, which can heavily impact the quality of resume reviews. So, a test that will compare the current prompt template string to a stored prompt template string (a snapshot) should be made. 
If there are changes and the version was not adjusted accordingly, this snapshot test should fail. If there are changes and an updated version, the test should pass. If there are no changes and no version change, this test should pass. If there are no changes and a version change, my assumption is that this test should still fail for incorrectly bumping up the version.

**Branch name:** test/37-snapshot-tests-for-prompt-templates

**Setup confirmation:** [Yes] App runs locally at localhost:5173

**Cohort ledger:** [N/A] Issue added to cohort ledger (I am a TF)