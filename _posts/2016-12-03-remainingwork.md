---
layout: post
title: Remaining artifice work
---

<script src="/js/mermaid.min.js"></script>
<div class="mermaid">
gantt
  dateFormat  YYYY-MM-DD
  title dRonin Artifice and Seppuku
  Get 1466-1470 merged         :done, merges, 2016-11-30,2016-12-02
  Rebase and update Sepp for RevB       :done, updateSepp, after merges, 1d
  Assembly RevB and initial bringup     :hardAssem, 2016-12-05, 2d
  Promo material creation   :promo, after hardAssem, 5d
  Shipping time    :shipRevB, after hardAssem, 2d
  MPL Test Matrix :mplRevBTestMatrix, after shipRevB, 4d
  Send to testers and get feedback    :feedback, after mplRevBTestMatrix, 10d
  Begin production:  production, after feedback, 25d
  Preorder window open :preorder, 2016-12-19, 1d
  Seppuku Documentation     :seppdocs, after shipRevB, 14d
  New autotune initial tests     :done, atinitial, 2016-11-30, 2016-12-01
  PR1450 merges   :done, pr1450merge, after atinitial, 1d
  Python PID model creation :pidmodel, after atinitial, 6d
  Autotune feedback from end users :atfeedback, after pidmodel, 7d
  GCS implementation and user feedback :gcsimpl, after atfeedback, 10d
  Code freeze and release test :freeze, after gcsimpl, 15d
  Artifice ship: after freeze, 1d
  First customer shipments: after production, 1d
</div>
