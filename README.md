# monthIdol
import java.util.ArrayList;
import java.util.Scanner;

class Main {
  public static void main(String[] args) {
    System.out.println("안녕하십니까! 짭간아이돌에 오신 것을 환영합니다!\n\n");
    System.out.println("제작자의 능력 부족으로 그룹의 멤버는 유동적인 구성이 힘듭니다.");
    System.out.println("제작하실 그룹의 멤버는 3명입니다.\n멤버의 이름을 입력해 주세요\n\n");

    Scanner scanner = new Scanner(System.in);
    System.out.println(">>멤버1: ");
    String member1 = scanner.nextLine();

    System.out.println(">>멤버2: ");
    String member2 = scanner.nextLine();

    System.out.println(">>멤버3: ");
    String member3 = scanner.nextLine();
    System.out.println("\n\n");
        
    ArrayList<String> sum = new ArrayList<> ();
    sum.add(member1);
    sum.add(member2);
    sum.add(member3);
    System.out.println(">>그룹의 멤버는 모두 " + sum.toString() + "입니다.");

    System.out.println(sum.toString() + "가 있는 그룹 명을 입력해 주세요.\n\n");
    Scanner tittle = new Scanner(System.in);
    String memtittle = tittle.nextLine();
    System.out.println(">>그룹명은 " + memtittle + "입니다.\n\n");

    System.out.println(memtittle + "이(가) 활동할 컨셉을 골라 주세요(숫자 입력)");
    System.out.println(">>1. 섹시\n>>2.큐티\n>>3.파워풀");
    Scanner scanner6 = new Scanner(System.in);
    String concept = scanner6.nextLine();
      if(concept.equals("1")){
      System.out.println(">>1번 섹시 컨셉을 고르셨습니다.\n활동곡 명을 입력해 주세요\n\n");
    }else {
      if(concept.equals("2")) {
        System.out.println(">>2번 큐티 컨셉을 고르셨습니다.\n활동곡 명을 입력해 주세요.\n\n");
      }else {
        if(concept.equals("3")){
          System.out.println(">>3번 파워풀 컨셉을 고르셨습니다.\n활동곡 명을 입력해 주세요.\n\n");
        }
      }
      }
      Scanner scanner3 = new Scanner(System.in);
      String song = scanner3.nextLine();
      System.out.println(">>" + memtittle + "이(가) 활동할 곡은 " + song + "입니다.\n\n\n");
      System.out.println("\n\n\n\n\n\n\n\n\n\n\n\n[일주일 후]\n\n\n");
      System.out.println("활동이 종료되었습니다.\n\n소속사로 반응 알림이 도착했습니다.\n아래 선택지 중 숫자를 입력해 주세요.");
      System.out.println(">>1\n>>2\n>>3");
      Scanner scanner5 = new Scanner(System.in);
      String yorb = scanner5.nextLine();
      if(yorb.equals("1")){
        System.out.println("\n\n\n\n[속보] " + memtittle + "의" + member2 + ", 소속사 선배 박박디라라와 핑크빛 연애...♥");
        System.out.println("\n\n큰일났습니다. 데뷔하자마자 같은 소속사 박박디라라와 사귀게 되었습니다.\n\n\n\n\n\n\n\nSAD ENDING");
      } else {
        if(yorb.equals("2")){
          System.out.println("\n\n\n\n[단독] 별안간 태국으로 떠난 " + member2 + "... '나는 잘못 태어나, 트랜스젠더로 다시 태어날 것' 충격");
          System.out.println("\n\n살다살다 이런 일이 일어날 줄은 몰랐습니다. 어안이 벙벙합니다. \n\n\n\n\n\n\n\nSAD ENDING");
        }else{
            System.out.println("\n\n\n\n[속보] 일냈다! 신예 루키즈 " +memtittle + ", 빌보드 핫 100 1위, 팝 스타 비욘세도 언급");
            System.out.println("축하합니다! 여기저기서 투자금이 물밀듯이 밀려와 자산금이 12조 4000억이 되었습니다.\n\n\n\n\n\n\n\nHAPPY ENDING");
        }
      }
}
}
