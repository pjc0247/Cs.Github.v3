Cs.Github.v3
====

Github.v3 API wrapping using [CsRestClient](https://github.com/pjc0247/CsRestClient).
<br>

Usage
----
```c#
var github =
  GithubAPIFactory.Create("YOUR_ID", "YOUR_PASSWORD");

Console.WriteLine(
    github.user.GetGists());
Console.WriteLine(
    github.GetRepo("pjc0247", "CsRestClient").GetReadme());
Console.WriteLine(
    github.GetGist("26ed50bea7aeee004d46").Star());
```

Remarks
----
* __CsRestClient__의 real-world 사용 예제를 보여주기 위한 프로젝트임
  * response도 죄다 string으로 옴
  * 모든 API를 다 래핑한게 아님
* [더좋은거](https://github.com/octokit/octokit.net)
