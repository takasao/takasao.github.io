{% assign is_ja = page.lang == 'ja' %}

{% if is_ja %}
<h2>プロフィール</h2>
<p>ここに日本語の自己紹介を記載してください。</p>

<h3>最近の活動</h3>
<ul>
  <li>プロジェクトや研究テーマ</li>
  <li>受賞・登壇</li>
  <li>他のページへの案内</li>
</ul>

<p>English page: <a href="{{ page.alt_url | default: '/en/' }}">English</a></p>
{% else %}
<h2>Profile</h2>
<p>Place your English bio here.</p>

<h3>Recent Highlights</h3>
<ul>
  <li>Key projects or research themes</li>
  <li>Awards or upcoming talks</li>
  <li>Links to other sections</li>
</ul>

<p>日本語: <a href="{{ page.alt_url | default: '/ja/' }}">日本語ページ</a></p>
{% endif %}
