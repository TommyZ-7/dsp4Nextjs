# dsp4Nextjs  
  
データサイエンスプロジェクト4秋学期制作物  
nextjs + shadchUI + sqliteで作成予定  
  
## dockerの共有方法  
---developper---  
1 docker build -t dsp4next .  
2 docker commit <container ID> dsp4nextjs:<version>  
3 docker save dsp4next:<version> > <filename(any)>.tar  
---server---  
4 docker load -i <filename>.tar  
5 docker build -p 3000:3000 dsp4next:<version>  
