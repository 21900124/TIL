# 2021-06-29

# 오늘의 문제점

STAR(simple tar)의 구현: 주된 3개의 기능(archive, list, extract)이 실행되는 것.
오늘 문제를 풀고 다른 사람들의 코드리뷰를 들으면서 내가 문제를 잘못이해하여 풀고 있다는 것을 알게 되었다. 사실 아카이브의 개념에 대한 이해가 가지 않았다. 
tar로 아카이브를 한다는 것은 폴더와 같은 것(?)을 만들어서 거기에 입력된 파일들을 써주는 것인지와 모든 내용(data)을 모두 써주는 것인지 이해가 되지 않았는데 다른 분들의 코드를 보면서 문제를 이해하였다.

# tar
tar는 파일의 용량을 줄이지 않고 하나로 묶어주는 명령어이다. 그 과정에서 대상이 되는 파일을 읽어서 파일의 크기와 이름을 써주고 입력이 디렉토리 경로인 경우 경로를 타고 들어가 파일을 열어서 읽은 다음 바로 아카이브 파일에 써준다.

# Today I learned

-시작하기 전에 문제를 정확하게 이해하고 포함해야 하는 기능들과 조건들을 정리해본다.

-조금의 코드라도 온전한 나의 생각과 논리를 바탕으로 써야하며 모르는 부분이 있다면 명확하게 파악하는 것이 중요하다.

-함수를 한 개 만들었다면 실행이 되는지 반드시 확인해보고 넘어가야한다.

-같이 공부하는 것의 중요성 : command line interface, test case를 만들때 다른 사람들이 한 것을 보면서 많은 도움이 되었다. 내가 미처 생각하지 못하고 넘어가는 부분들을 놓치지 않을 수 있었고 코드를 짤 때도 내가 올바른 방향으로 코드를 짜고 있는지 확인할 수 있다.

-코드의 실행을 설명하는 주석은 달지 않는다.
