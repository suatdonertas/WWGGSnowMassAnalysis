# WWGGSnowMassAnalysis — Future Collider Sensitivity Study

Analysis code for a Snowmass study — the multi-year U.S. particle physics community
process that sets priorities for future collider experiments — projecting how sensitive
a future higher-luminosity or higher-energy collider would be to the HH → WWγγ
di-Higgs channel.

## The problem, in plain terms

Rather than analyzing data that already exists, this work asks a forward-looking
question: *if we build a bigger or longer-running collider, how much better would our
ability to detect this rare process actually get?* This requires simulating expected
signal and background yields under different future-collider scenarios and projecting
statistical sensitivity — essentially a large-scale "what-if" analysis used to justify
and shape real, multi-billion-dollar scientific infrastructure decisions.

## Technical approach

- Builds on the classification and significance-estimation pipeline from
  [`DNN_HHWWGG`](https://github.com/sutipati/DNN_HHWWGG), applied to projected future
  datasets rather than existing collision data
- Projects statistical sensitivity under multiple future-collider luminosity/energy
  assumptions, requiring careful handling of scaled and reweighted simulated samples
- Same distributed batch-computing approach (Slurm-based HPC processing) as the parent
  analysis, applied at the scale needed for community-wide projection studies

## Why this matters beyond physics

This is fundamentally a **long-horizon scenario-planning and sensitivity-modeling**
exercise — quantifying the expected value of a future investment before it's made,
under multiple assumptions about how that investment might play out. The same
underlying skill (running structured simulations across many scenarios, then
statistically summarizing what each would mean) shows up anywhere decisions need to be
made under uncertainty about a future system that doesn't exist yet.

