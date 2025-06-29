<ul>
<li>This simple simulation shows how random sampling can help estimate mathematical constants like &pi;.</li>
<li><b>The more points you use, the more accurate your estimate becomes.</b></li>
<li>The method visually and mathematically demonstrates how probability and geometry are connected.</li>
<li>Monte Carlo simulations are powerful tools for solving problems that are hard to calculate directly, using randomness and statistics.</li>
</ul>
<h3>Manual Monte Carlo Probability Calculation for π Estimation</h3>

<p>Let's compute with <b>4 example points</b> in the unit square [0,1]×[0,1]:</p>

<table border="1" style="border-collapse: collapse; width: 100%;">
  <tr>
    <th>Point</th>
    <th>Coordinates</th>
    <th>Check: (x-0.5)² + (y-0.5)² ≤ 0.25</th>
    <th>Inside Circle?</th>
  </tr>
  <tr>
    <td>1</td>
    <td>(0.6, 0.6)</td>
    <td>(0.1)² + (0.1)² = 0.02 ≤ 0.25</td>
    <td>✅ Yes</td>
  </tr>
  <tr>
    <td>2</td>
    <td>(0.7, 0.3)</td>
    <td>(0.2)² + (-0.2)² = 0.08 ≤ 0.25</td>
    <td>✅ Yes</td>
  </tr>
  <tr>
    <td>3</td>
    <td>(0.2, 0.9)</td>
    <td>(-0.3)² + (0.4)² = 0.25 ≤ 0.25</td>
    <td>✅ Yes</td>
  </tr>
  <tr>
    <td>4</td>
    <td>(0.9, 0.8)</td>
    <td>(0.4)² + (0.3)² = 0.25 > 0.25</td>
    <td>❌ No</td>
  </tr>
</table>

<h4>Calculation:</h4>
<ol>
  <li><b>Points inside circle:</b> 3</li>
  <li><b>Total points:</b> 4</li>
  <li><b>Estimated probability:</b><br>
      <div style="text-align:center; margin:10px">
        <sup>Points inside</sup>&frasl;<sub>Total points</sub> = <sup>3</sup>&frasl;<sub>4</sub> = 0.75
      </div>
  </li>
  <li><b>π estimate:</b><br>
      <div style="text-align:center; margin:10px">
        π ≈ 4 × <sup>3</sup>&frasl;<sub>4</sub> = 3.0
      </div>
  </li>
</ol>

<h4>Key Observations:</h4>
<ul>
  <li>Actual probability = π/4 ≈ 0.7854</li>
  <li>Manual estimate (0.75) has error due to small sample size</li>
  <li>Accuracy improves with more points (Law of Large Numbers)</li>
</ul>

<h4>Conclusion:</h4>
<p>This verifies π ≈ 4 × (circle points / total points). The method demonstrates how randomness approximates deterministic constants, with accuracy increasing with sample size.</p>
