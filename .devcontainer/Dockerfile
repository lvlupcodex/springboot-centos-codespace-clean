FROM centos:7

# Instalación de Java, Maven, Git y herramientas esenciales
RUN yum update -y && \
    yum install -y java-17-openjdk-devel git maven wget unzip && \
    yum clean all

ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk
ENV PATH=$JAVA_HOME/bin:$PATH

# Carpeta de trabajo por defecto
WORKDIR /workspace

CMD ["/bin/bash"]