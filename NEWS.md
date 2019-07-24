# elmr 0.5.6

* new `prune_twigs()` function that removes twigs less than a threshold length.
  Useful thing to do as part of preparing `dotprops()` objects for `nblast()`.
* Fix strange arrows in `plot3d.ngraph()` (#45)
* Allow `open_fafb()` to specify a different CATMAID server (including via a
  `catmaid_connection()` object) (#44)
* Teach `nblast_fafb()` to prune twigs by default
* fix hitherto silent bugs revealed by R 3.6

# elmr 0.5.5

* teach `open_fafb()` to make many URLs at once e.g. for results of tagged_details
  (#41)

# elmr 0.5.4

* add `plot3d.ngraph()` (shows directed graph in 3d)
* fix `simplify_neuron()` when spine has 1 branch only (#40)
* vignette tweaks

# elmr 0.5.3

* teach `simplify_neuron()` to handle the inverse as well (#38)
* change IVLP -> WED in FAFBNP surfaces as well as FAFB14NP (#35)
* teach fetchn_fafb to work even if FAFB is given as the reference brain (#39)

# elmr 0.5.2

* teach `simplify_neuron()` to handle arbitrary number of branch points (#37)
* minor doc fixes

# elmr 0.5.1

* teach `distal_to()` to handle multiple input nodes
* add `simplify_neuron function()` to make neuron with just one branchpoint
* fix `summarise_contributions()` for 'synapses' (#34)
* change IVLP -> WED in FAFBNP surfaces (#35)
* fix `stitch_neurons()` for latest nat 1.9 prerelease (#36)

# elmr 0.5

* switch to FAFB14 as the default EM assembly
* provide default objects (FAFB, FAFB.surf, FAFBNP.surf) that will always point
  to current assembly.
* fix bug in `distal_to()` (#31)
* doc improvements for `distal_to()`

# elmr 0.4.2

* update to 170303_ELM_landmarks_v14 landmarks (including transforming surfaces)
* first version of `unspike()` function
* new vignette - making meshes programmatically
* insist on nat >= 1.8.8
* `fetchn_fafb()`/`nblast_fafb()` can take pre-downloaded neuronlist
* teach `unspike()` to keep connectors/soma (#29)

# elmr 0.4.1

* Add functions to summarise tracer effort

# elmr 0.4

* switch FAFB13-JFRC2013 transform to 170211_new_ELM_landmarks_v7.csv
  (71 landmarks more evenly spaced on both sides of the brain)
* update FAFB13 and FAFB13NP surface objects accordingly
* fix `open_fafb()` after change in stack id handling
* add landmarks vignette

# elmr 0.3

* make `nblast_fafb()` parallelised by default
* give `open_fafb()` arguments for selecting neuron/nodes (#24)
* add FAFB13 brain and neuropil surface objects
* complete switch to FAFB13 assembly (vignettes etc)
* fix `open_fafb()` for v13 (#23)

# elmr 0.2.1

* teach `nblast_fafb()` to cope with db length <100 (#22)

# elmr 0.2

* switch to FAFB13 as default template brain
* much new functionality including transforming between template brains via
  `xform_brain()`
* `nblast_fafb()` for searches

# elmr 0.1

* first version
