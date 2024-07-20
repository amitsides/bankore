FROM centos:7
RUN yum update -y && \
    yum install -y wget gcc make ncurses-devel
RUN wget https://sourceforge.net/projects/gnucobol/files/gnucobol/3.1/gnucobol-3.1.tar.gz && \
    tar -xvf gnucobol-3.1.tar.gz && \
    cd gnucobol-3.1 && \
    ./configure && \
    make && \
    make install && \
    cd .. && \
    rm -rf gnucobol-3.1 gnucobol-3.1.tar.gz
WORKDIR /app
COPY your_cobol_program.cob .
RUN cobc -x -o your_cobol_program your_cobol_program.cob
CMD ["./your_cobol_program"]