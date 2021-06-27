# Trabajo_de_embrage
#Datos del ejercicio
m=1 #[kg]
R1=0.3 #[m]
tworad=0.4 #[m]
#Ecuaciones y aálisis
vangular=np.arange(0,201,1)
T=m*R1*((vangular*((np.pi)/30))**2)
#plot
fig=px.line(x=vangular,y=T,labels={'x':'Velocidad Angular [rad/s]','y':'Tension[N]'},title="Tension VS velocidad angular")
fig.show()
