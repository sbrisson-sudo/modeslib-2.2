add_executable(yannos
    yannos.f90
    def_gparam.f90   
    module_com_minos.f90 
    module_modele.f90 
    util_minos.f90  
    module_neominos.f90  
    module_spline.f90 
    sub_minosa4.f
    nrutil.f90  
    nrtype.f90   
    yannos_flag.f90 
    layer.f90 
    )

add_executable(yannos_MPI
    yannos_MPI.f90
    def_gparam.f90   
    module_com_minos.f90 
    module_modele.f90 
    util_minos.f90  
    module_neominos.f90  
    module_spline.f90 
    sub_minosa4.f
    nrutil.f90  
    nrtype.f90   
    yannos_flag.f90 
    layer.f90 
    )

target_link_libraries(yannos_MPI
    PUBLIC MPI::MPI_Fortran
)
