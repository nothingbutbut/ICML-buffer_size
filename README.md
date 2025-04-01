# ER Decay compared to smaller buffer sizes
<p>
  <img src="https://github.com/nothingbutbut/ICML-buffer_size/blob/main/Ant-v4-performance.png" alt="Ant-v4" style="width:32%; float:left; margin-right:1%;">
  <img src="https://github.com/nothingbutbut/ICML-buffer_size/blob/main/humanoid-walk-performance.png" alt="humanoid-walk" style="width:32%; float:left; margin-left:1%;">
  <img src="https://github.com/nothingbutbut/ICML-buffer_size/blob/main/dog-walk-performance.png" alt="dog-walk" style="width:32%; float:left; margin-left:1%;">
</p>
<p style="clear:both; font-size:18px; margin-top:20px;">
  This experiment was conducted to compare the performance of ER decay with smaller buffer sizes. We use normal SAC as algorithm without any other modifications to exclude the effect of other factors. We compare ones with buffer size of 50k, 100k, 250k and 500k to ER decay with full buffer size of 1M. The results show that ER decay with full buffer size outperforms all the smaller buffer sizes in terms of sample efficiency and final performance. The results are shown in the figure above. This suggests that While ER Decay introduces more "on-policy" characteristics, it also retains older transitions, preventing forgetting and improving final performance.
  All experiments are conducted with 6 seeds.
</p>
