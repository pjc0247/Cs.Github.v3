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
* __CsRestClient__�� real-world ��� ������ �����ֱ� ���� ������Ʈ��
  * response�� �˴� string���� ��
  * ��� API�� �� �����Ѱ� �ƴ�