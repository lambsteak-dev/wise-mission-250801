package com.back;

import java.util.Scanner;
import java.util.ArrayList;
import java.util.List;

public class Main {
public static void main(String[] args) {
test1(args);
test2(args);
test3(args);
test4(args);
test5(args);
test6(args);
test7(args);
test8(args);


    }
    public static void test8(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");
        int n = 0;
        List<String> saying = new ArrayList<>();
        List<String> auth = new ArrayList<>();
        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                saying.add(sc.nextLine());
                System.out.print("작가 : ");
                auth.add(sc.nextLine());
                n++;
                System.out.println("%d번 명언이 등록되었습니다.".formatted(n));
            } else if (command.equals("종료")) {
                break;
            } else if (command.equals("목록")) {
                System.out.println("번호 / 작가 / 명언 ");
                System.out.println("----------------------");
                for (int i = n; i > 0; i--) {
                    if (saying.get(i - 1) != null) {
                        System.out.println("%d / %s / %s ".formatted(i,auth.get(i-1),saying.get(i-1)));                    }
                }

            } else if (command.startsWith("삭제?id=")) {

                String a = command.substring(6);
                int b = Integer.parseInt(a);
                String c = saying.get(b - 1);
                if (c == null) {
                    System.out.println("%d번 명언은 존재하지 않습니다.".formatted(b));
                } else {
                    saying.set(b - 1, null);
                    auth.set(b - 1, null);
                    System.out.println("%d번 명언이 삭제되었습니다.".formatted(b));
                }
            } else if (command.startsWith("수정?id=")) {

                String a = command.substring(6);
                int b = Integer.parseInt(a);
                String c = saying.get(b - 1);
                if (c == null) {
                    System.out.println("%d번 명언은 존재하지 않습니다.".formatted(b));
                } else {
                    System.out.println("명언(기존) : " + c);
                    System.out.print("명언 : ");
                    saying.set(b - 1, sc.nextLine());
                    System.out.println("작가(기존) : " + auth.get(b - 1));
                    System.out.print("작가 : ");
                    auth.set(b - 1, sc.nextLine());

                }
            }
        }
    }

    public static void test7(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");
        int n = 0;
        List<String> saying = new ArrayList<>();
        List<String> auth = new ArrayList<>();
        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                saying.add(sc.nextLine());
                System.out.print("작가 : ");
                auth.add(sc.nextLine());
                n++;
                System.out.println("%d번 명언이 등록되었습니다.".formatted(n));
            } else if (command.equals("종료")) {
                break;
            } else if (command.equals("목록")) {
                System.out.println("번호 / 작가 / 명언 ");
                System.out.println("----------------------");
                for (int i = n; i > 0; i--) {
                    if (saying.get(i - 1) != null) {
                        System.out.println("%d / %s / %s ".formatted(i,auth.get(i-1),saying.get(i-1)));                    }
                }

            } else if (command.startsWith("삭제?id=")) {

                String a = command.substring(6);
                int b = Integer.parseInt(a);
                String c = saying.get(b - 1);
                if (c == null) {
                    System.out.println("%d번 명언은 존재하지 않습니다.".formatted(b));
                } else {
                    saying.set(b - 1, null);
                    auth.set(b - 1, null);
                    System.out.println("%d번 명언이 삭제되었습니다.".formatted(b));
                }
            }
        }
    }


    public static void test6(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");
        int n = 0;
        List<String> saying = new ArrayList<>();
        List<String> auth = new ArrayList<>();
        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                saying.add(sc.nextLine());
                System.out.print("작가 : ");
                auth.add(sc.nextLine());
                n++;
                System.out.println("%d번 명언이 등록되었습니다.".formatted(n));
            } else if (command.equals("종료")) {
                break;
            } else if (command.equals("목록")) {
                System.out.println("번호 / 작가 / 명언 ");
                System.out.println("----------------------");
                for (int i = n; i > 0; i--) {
                    if (saying.get(i - 1) != null) {
                        System.out.println("%d / %s / %s ".formatted(i,auth.get(i-1),saying.get(i-1)));
                    }
                }

            } else if (command.startsWith("삭제?id=")) {

                String a = command.substring(6);
                int b = Integer.parseInt(a);
                String c = saying.get(b - 1);
                saying.set(b - 1, null);
                auth.set(b - 1, null);
                System.out.println("%d번 명언이 삭제되었습니다.".formatted(b));
                }
            }
        }


    public static void test5(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");
        int n = 0;
        List<String> saying = new ArrayList<>();
        List<String> auth = new ArrayList<>();
        while (true) {
            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                saying.add(sc.nextLine());
                System.out.print("작가 : ");
                auth.add(sc.nextLine());
                n++;
                System.out.println("%d번 명언이 등록되었습니다.".formatted(n));
            } else if (command.equals("종료")) {
                break;
            } else if (command.equals("목록")) {
                System.out.println("번호 / 작가 / 명언 ");
                System.out.println("----------------------");
                for (int i = n; i > 0; i--) {
                    if (saying.get(i - 1) != null) {
                        System.out.println("%d / %s / %s ".formatted(i, auth.get(i - 1), saying.get(i - 1)));
                    }
                }

            }
        }
    }

    public static void test4(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");
        int n = 0;
        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                sc.nextLine();
                System.out.print("작가 : ");
                sc.nextLine();
                n++;
                System.out.println("%d번 명언이 등록되었습니다.".formatted(n));
            } else if (command.equals("종료")) {
                break;
            }
        }
    }

    public static void test3(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");

        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                sc.nextLine();
                System.out.print("작가 : ");
                sc.nextLine();

                System.out.println("1번 명언이 등록되었습니다.");
            } else if (command.equals("종료")) {
                break;
            }
        }
    }

    public static void test2(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");

        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("등록")) {
                System.out.print("명언 : ");
                sc.nextLine();
                System.out.print("작가 : ");
                sc.nextLine();
            } else if (command.equals("종료")) {
                break;
            }
        }
    }

    public static void test1(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("==명언 앱 ==");

        while (true) {

            System.out.print("명령) ");
            String command = sc.nextLine();//입력값 받기
            if (command.equals("종료")) {
                break;
            }
        }
    }
}
