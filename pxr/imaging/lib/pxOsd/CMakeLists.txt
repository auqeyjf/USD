set(PXR_PREFIX pxr/imaging)
set(PXR_PACKAGE pxOsd)

pxr_shared_library(pxOsd
    LIBRARIES
        tf
        gf
        vt
        ${OPENSUBDIV_LIBRARIES}

    INCLUDE_DIRS
        ${OPENSUBDIV_INCLUDE_DIR}

    PUBLIC_CLASSES
        meshTopology
        refinerFactory
        refinerCache
        stencilPerVertex
        subdivTags
        tokens
        uniformEvaluator

)
