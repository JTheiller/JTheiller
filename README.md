<!--
**JTheiller/JTheiller** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.


Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
<p align="left">
<img src="https://raw.githubusercontent.com/JTheiller/JTheiller/main/assets/contribution.png" alt="c" width = "100%" heigth: "auto" max-width = "100%"/> 
<a href="https://github.com/JTheiller"> <img align="left" src="https://github-readme-stats.vercel.app/api/top-langs/?username=JTheiller" /></a>
<a href="https://github.com/JTheiller"> <img src="https://github-readme-stats.vercel.app/api?username=JTheiller&count_private=true&show_icons=true&include_all_commits=true" /></a>  
</p>
<p align="left">
<code><img height="20" src="https://raw.githubusercontent.com/file-icons/icons/master/svg/Delphi.svg"></code>
<code><img height="20" src="https://raw.githubusercontent.com/file-icons/icons/master/svg/Pascal.svg"></code>
<code><img height="20" src="https://raw.githubusercontent.com/file-icons/icons/master/svg/VSCode.svg"></code>
</p>
<br><br><br><br><br>
<p align="center">
<a href="https://github.com/JTheiller"> <img src="http://chart.apis.google.com/chart?cht=qr&chl=joathan theiller&chs=120x120" /></a> <br>
<img src="https://raw.githubusercontent.com/github/explore/80688e429a7d4ef2fca1e82350fe8e3517d3494d/topics/git/git.png" alt="GIT" width="45" height="45"/> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original-wordmark.svg" alt="docker" width="45" height="40"/> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" alt="c" width="40" height="40"/> 
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/cplusplus/cplusplus-original.svg" alt="cplusplus" width="40" height="40"/> 
</p>
<p align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/windows8/windows8-original.svg" alt="windows" width="40" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" alt="linux" width="40" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/android/android-original-wordmark.svg" alt="android" width="40" height="40"/>
</p>
<p align="center">
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" alt="html5" width="40" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" alt="css3" width="40" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/angularjs/angularjs-original.svg" alt="docker" width="45" height="40"/>
<img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" alt="javascript" width="40" height="40"/>
</p>
<p align="center">
<a href="https://github.com/JTheiller/JTheiller"><img src="https://img.shields.io/github/stars/JTheiller/JTheiller" alt="Stars Badge"/></a>
<a href="https://github.com/JTheiller/JTheiller/network/members"><img src="https://img.shields.io/github/forks/JTheiller/JTheiller" alt="Forks Badge"/></a>
<a href="https://github.com/JTheiller/JTheiller/pulls"><img src="https://img.shields.io/github/issues-pr/JTheiller/JTheiller" alt="Pull Requests Badge"/></a>
<a href="https://github.com/JTheiller/JTheiller/issues"><img src="https://img.shields.io/github/issues/JTheiller/JTheiller" alt="Issues Badge"/></a>
<a href="https://github.com/JTheiller/JTheiller/graphs/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/JTheiller/JTheiller?color=2b9348"></a>
<a href="https://github.com/JTheiller/JTheiller/blob/master/LICENSE"><img src="https://img.shields.io/github/license/JTheiller/JTheiller?color=2b9348" alt="License Badge"/></a>
<a href="https://github.com/JTheiller"> <img src="https://visitor-badge.laobi.icu/badge?page_id=JTheiller" /></a><br>
<a href="https://github.com/JTheiller"> <img src="https://img.shields.io/github/repo-size/JTheiller/JTheiller" /></a><br>
</p>
<p align="center">
<a href="https://gitstats.me/JTheiller"> <img src="https://img.shields.io/badge/-JTheiller-black?style=flat&labelColor=black&logo=github&logoColor=white" /></a>
</p>

```pascal
program ProjectForeverAlive;

{$APPTYPE CONSOLE}

uses
  SysUtils;

type
  IDeveloper = interface['{4E9E0CB0-49AC-4455-9CFA-D5E2724E9B80}']
  end;

  IMachine = interface['{9C45ADC2-08C2-4D9E-BEA3-BEE87AF7A718}']
  end;

  IHumam = interface(IMachine)['{BF7B51A1-2A23-4E9C-8FE4-B4EDB08BFF05}']
  function IsAlive: Boolean;
  end;

  THumam = class(TInterfacedObject, IHumam, IMachine, IDeveloper)
  private
    FName: String;
  public
    constructor Create(AName: String);
    procedure Start;
    function IsAlive: Boolean;
    property Name: String read FName;
  end;

{ THuman }

function THumam.IsAlive: Boolean;
const
  Forever = True;
begin
  Result := Forever;
end;

procedure THumam.Start;
begin
  while IsAlive do
  begin
    WriteLn( Format('%s: %s: %s',[FormatDateTime('YYYY/MM/DD - HH:MM:SS',Now), Name, 'another new idea...']) );
  end;
end;

constructor THumam.Create(AName: String);
begin
  inherited Create;
  FName := AName;
end;

begin
  THumam.Create('Joathan Theiller').Start;
end.
```
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CIEvolution-blue"></code>
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CIMagazine-blue"></code>
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CIDOCe-blue"></code>
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CIFactory-blue"></code>
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CIAgency-blue"></code>
<code><img height="20" src="https://img.shields.io/badge/Project-ConceitoTec--CISyncDB-blue"></code>
