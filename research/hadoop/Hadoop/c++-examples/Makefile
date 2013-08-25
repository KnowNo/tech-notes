HADOOP_INSTALL=/home/zhongxia/Software/hadoop-0.20.2+737
PLATFORM=Linux-amd64-64

CC = g++
CPPFLAGS = -m64 -I$(HADOOP_INSTALL)/c++/$(PLATFORM)/include

wordcount: wordcount.cpp
	$(CC) $(CPPFLAGS) $< -Wall -L$(HADOOP_INSTALL)/c++/$(PLATFORM)/lib -lhadooppipes -lhadooputils -lpthread -lcrypto -lssl -g -O2 -o $@

