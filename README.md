//结构体学习
#include<stdio.h>

struct xs      //定义结构体类型（  struct xs -- int / char ）
{
	char name1[6];
	int studentname1;
	char sex1[4];
	char telephone1[12];
};

typedef struct xsxx
{
	char name2[8];
	char zuoyou[20];
	char sex2[8];
	char telephone2[12];
}结构体;

int main()
{
	struct xs x = { "李华",20230301,"女","15166668888"};    //创建一个结构体变量并进行初始化
	printf("姓名：%s \n学号：%d \n性别：%s \n电话：%s \n", x.name1, x.studentname1, x.sex1, x.telephone1);
	结构体 xues = { "坤坤","再多看一眼就会爆炸","未知","坤你太美" };
	printf("姓名：%s \n座右铭：%s \n性别：%s \n电话：%s \n", xues.name2, xues.zuoyou, xues.sex2, xues.telephone2);
	return 0;
}
