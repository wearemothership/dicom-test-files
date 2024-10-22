dclunie@dclunie.com

2004/08/26

This set consists of a collection of medical images in both
uncompressed form, and compressed with various lossless
and lossy compression schemes defined by the DICOM standard.

These include JPEG lossless (JPLL) and lossy (JPLY), JPEG-LS in
lossless (JLSL) and near-lossless modes (JLSN), and JPEG 2000
reversible (J2KR) and irreversible (J2KI).

Not all the images have been compressed using all schemes and
modes; in particular the color images have been compressed using
JPEG 2000 only, and since the JPEG lossy process only supports
12 bit unsigned images, those images with an actual dynamic range
outside that range have not been JPEG lossy compressed.

No effort has been made to align the target bit-rates (compression
ratios) of the various lossy compressors, since the objective
is to provide sample images to test and demonstrate implementation,
not to compare the efficacy of one scheme with another. While one
can obviously compare the effectiveness of lossless compression
by looking at the file sizes, the small number of images and diversity
of modalities used make such a comparison fairly meaningless. For
interest, the file sizes are as follows:

IMG      UNC    J2KI     J2KR     JLSL    JLSN     JPLL    JPLY
CT1   530632   14156   180916   170882   91682   210532
CT2   525920    6830   121356   117288   51260   166126
MG1 28582296 2680914 12233370 12022866 6573186 12834242 2823426
MR1   525926    9012   238756   231576  128998   262134   71948
MR2  2098988  113550   589212   599990  281722   779708  120390
MR3   533746   12430   122274   127780   73956   173104   46688
MR4   526146   12394   114900   118788   47878   155410   17792
NM1   527066    3308    89958    92020   32230   118986    9844
RG1  7200056  676846  4285194  4197660 2765596  4445624
RG2  7534130  707654  1660380  1672994  699292  2162496  211568
RG3  6196600  207152   832104   849008  290040  1398846   94084
SC1 10187866  781702  2444182  2154188 1102592  3112030  768386
US1   922878   59140   153760
VL1  1103386   70266   297182
VL2  1103384   70304   308850
VL3  1103396   70260   304298
VL4 12475634  781134  5854298
VL5 26754534 1673714 15112658
VL6  1103396   70036   612400
XA1  2098206  109340   403336   391932  131822   495626   44166

The compressed images are encapsulated as per the standard
requirements in PS 3.5; even though all the images are single
frame in some cases the compressed bitstream is fragmented
into multiple items.

The codecs used were:

- for JPEG, the Stanford PVRG codec
- for JPEG-LS, the dicom3tools rawnjl2 codec
- for JPEG 2000, the Kakadu codec

The following images are contained in the set, as described
by the accompanying DICOMDIR:

PATIENT CompressedSamples^XA1 20XA1
        STUDY 20XA1  20030612 185520 
                SERIES 1 XA
                        IMAGE 1
                         -> IMAGES\REF\XA1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\XA1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\XA1_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\XA1_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\XA1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\XA1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\XA1_J2KI
PATIENT CompressedSamples^VL6 19VL6
        STUDY 19VL6  20030612 185520 Stomach Body Biopsy - Micro
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL6_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL6_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL6_J2KI
PATIENT CompressedSamples^VL5 18VL5
        STUDY 18VL5  20030612 185520 Whole Prostate
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL5_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL5_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL5_J2KI
PATIENT CompressedSamples^VL4 17VL4
        STUDY 17VL4  20030612 185520 Fundoscopy
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL4_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL4_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL4_J2KI
PATIENT CompressedSamples^VL3 16VL3
        STUDY 16VL3  20030612 185520 Arterio-venous Malformation
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL3_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL3_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL3_J2KI
PATIENT CompressedSamples^VL2 15VL2
        STUDY 15VL2  20030612 185520 Prepyloric Ulcer
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL2_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL2_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL2_J2KI
PATIENT CompressedSamples^VL1 14VL1
        STUDY 14VL1  20030612 185520 Barretts Esophagus
                SERIES 1 OT
                        IMAGE 1
                         -> IMAGES\REF\VL1_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\VL1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\VL1_J2KI
PATIENT CompressedSamples^US1 13US1
        STUDY 13US1  20030612 185520 
                SERIES 1 US
                        IMAGE 1
                         -> IMAGES\REF\US1_UNC
                        IMAGE 2
                         -> IMAGES\J2KR\US1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\US1_J2KI
PATIENT CompressedSamples^SC1 12SC1
        STUDY 12SC1  20030612 185520 
                SERIES 1 CT
                        IMAGE 1
                         -> IMAGES\REF\SC1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\SC1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\SC1_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\SC1_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\SC1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\SC1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\SC1_J2KI
PATIENT CompressedSamples^RG3 11RG3
        STUDY 11RG3 FUJI95706 20030612 185520 Non-ossifying fibroma of distal tibia
                SERIES 1 CR
                        IMAGE 1
                         -> IMAGES\REF\RG3_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\RG3_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\RG3_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\RG3_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\RG3_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\RG3_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\RG3_J2KI
PATIENT CompressedSamples^RG2 10RG2
        STUDY 10RG2  20030612 185520 HIP JOINT
                SERIES 1 CR
                        IMAGE 1
                         -> IMAGES\REF\RG2_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\RG2_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\RG2_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\RG2_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\RG2_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\RG2_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\RG2_J2KI
PATIENT CompressedSamples^RG1 9RG1
        STUDY 9RG1 exam Number 20030612 185520 THORAX
                SERIES 1 CR
                        IMAGE 1
                         -> IMAGES\REF\RG1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\RG1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\RG1_JLSL
                       IMAGE 4
                         -> IMAGES\JPLL\RG1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\RG1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\RG1_J2KI
PATIENT CompressedSamples^NM1 8NM1
        STUDY 8NM1  20030612 185520 Whole Body Bone
                SERIES 1 NM
                        IMAGE 1
                         -> IMAGES\REF\NM1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\NM1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\NM1_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\NM1_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\NM1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\NM1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\NM1_J2KI
PATIENT CompressedSamples^MR4 7MR4
        STUDY 7MR4  20030612 185520 BRAIN
                SERIES 1 MR
                        IMAGE 1
                         -> IMAGES\REF\MR4_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\MR4_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\MR4_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\MR4_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\MR4_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\MR4_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\MR4_J2KI
PATIENT CompressedSamples^MR3 6MR3
        STUDY 6MR3  20030612 185520 e+1 KNEE-RT.
                SERIES 1 MR
                        IMAGE 1
                         -> IMAGES\REF\MR3_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\MR3_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\MR3_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\MR3_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\MR3_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\MR3_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\MR3_J2KI
PATIENT CompressedSamples^MR2 5MR2
        STUDY 5MR2  20030612 185520 SHOULDER
                SERIES 1 MR
                        IMAGE 1
                         -> IMAGES\REF\MR2_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\MR2_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\MR2_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\MR2_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\MR2_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\MR2_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\MR2_J2KI
PATIENT CompressedSamples^MR1 4MR1
        STUDY 4MR1  20030612 185520 
                SERIES 1 MR
                        IMAGE 1
                         -> IMAGES\REF\MR1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\MR1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\MR1_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\MR1_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\MR1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\MR1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\MR1_J2KI
PATIENT CompressedSamples^MG1 3MG1
        STUDY 3MG1  20030612 185520 Malignant mass with micro-calcifications
                SERIES 1 RG
                        IMAGE 1
                         -> IMAGES\REF\MG1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\MG1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\MG1_JLSL
                        IMAGE 5
                         -> IMAGES\JPLY\MG1_JPLY
                        IMAGE 4
                         -> IMAGES\JPLL\MG1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\MG1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\MG1_J2KI
PATIENT CompressedSamples^CT2 2CT2
        STUDY 2CT2  20030612 185520 
                SERIES 1 CT
                        IMAGE 1
                         -> IMAGES\REF\CT2_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\CT2_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\CT2_JLSL
                        IMAGE 4
                         -> IMAGES\JPLL\CT2_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\CT2_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\CT2_J2KI
PATIENT CompressedSamples^CT1 1CT1
        STUDY 1CT1  20030612 185520 e+1
                SERIES 1 CT
                        IMAGE 1
                         -> IMAGES\REF\CT1_UNC
                        IMAGE 7
                         -> IMAGES\JLSN\CT1_JLSN
                        IMAGE 6
                         -> IMAGES\JLSL\CT1_JLSL
                        IMAGE 4
                         -> IMAGES\JPLL\CT1_JPLL
                        IMAGE 2
                         -> IMAGES\J2KR\CT1_J2KR
                        IMAGE 3
                         -> IMAGES\J2KI\CT1_J2KI

The set of uncompressed images are those that were originally
supplied to ISO/IEC JTC1/SC29/WG1 for the purpose of informally
evaluating the effect of proposed JPEG 2000 schemes on image
quality. An updated version of the original description of
the images supplied to JTC1/SC29/WG1 follows ...

The images contain no patient identifying information.

They were initially obtained from various publically available
collections of images, including NEMA DICOM demonstrations
and public web servers, as well as some images specifically
solicited for the purpose of testing compression. The original
sources were:

- CT1,MR3,NM1,US1,XA1: GE
- CT2,MR1: Toshiba
- MR2,MR4,RG1: Philips
- RG2,RG3: Fuji
- MG1: USF (http://marathon.csee.usf.edu/Mammography/Database.html)
- SC1: Cemax (now Kodak)
- VL1,VL2,VL3: ASGE
- VL4: AAO (Hildebrand)
- VL5,VL6: CAP (Balis)

They are intended to be a representative set of the broad
range of different types of medical images. They may not
necessarily be particularly challenging or unusual and may not
contain any particularly subtle abnormalities, so should
not be assumed to be critical tests of a compression
scheme nor imply any likely usefulness from a diagnostic
point of view. The decision to use a lossy compression
scheme for medical applications may require a more rigorous
observer-performance study of a carefully selected set to
test a particular diagnostic task.

The uncompressed images are "dual-personality" in the sense that
they are both DICOM and TIFF images.

Images are all encoded as standard DICOM Image Storage SOP Classes;
the Visible Light and Mammography images are stored as Secondary Capture,
since more specific SOP Classes were not defined at the time that
these images were originally created.

Non-medical users may find it more convenient to extract
the pixel data from the images using a conventional TIFF
reader, rather than a DICOM reader. Be aware that some of
the images, including the CT and some of the MR images,
contained signed data, and hence will "look strange". It
is expected that the results of the compress/decompress
cycle will result in data of the same form as the original
and will be evaluated visually using medical software
that "knows" about signed data, ie. don't try to fix
what these "look like" before compressing them !

The following uncompressed reference images are present:

Image                     File          Pixel Data     Rows  Cols Bits Samples Zero Order
                                      Bytes   Offset                            Entropy

CT Lung Contrast         CT1_UNC      524288   6176     512   512  16     1     8.20914
CT Brain Contrast        CT2_UNC      524288   1426     512   512  16     1     6.8012
Mammogram                MG1_UNC    28580992   1186    4664  3064  12     1     10.561
MR Posterior Fossa       MR1_UNC      524288   1430     512   512  16     1     10.083
MR Shoulder              MR2_UNC     2097152   1728    1024  1024  12     1     6.89806
MR Knee                  MR3_UNC      524288   9272     512   512  16     1     6.30807
MR Brain                 MR4_UNC      524288   1748     512   512  12     1     6.03216
NM Bonescan              NM1_UNC      524288   2632    1024   256  16     1     3.99372
Chest X-Ray              RG1_UNC     7198310   1570    1955  1841  15     1     13.7073
Hip Joint                RG2_UNC     7532800   1134    2140  1760  10     1     7.20069
Bone Lesion Leg          RG3_UNC     6195200   1202    1760  1760  10     1     6.62469
US Color Tissue Doppler  US1_UNC      921600   1044     480   640   8     3     3.11635
XA Neuroangiogram        XA1_UNC     2097152    936    1024  1024  10     1     6.53488
Scanned Film CT Brain    SC1_UNC    10186752    880    2487  2048  12     1     5.75373
GI Endoscopy Esophagus   VL1_UNC     1102248    894     486   756   8     3     2.66609
GI Endoscopy Stomach     VL2_UNC     1102248    890     486   756   8     3     2.99886
GI Endoscopy Colon       VL3_UNC     1102248    900     486   756   8     3     2.55583
Retinal Fundoscopy       VL4_UNC    12474504    870    1868  2226   8     3     4.32233
Pathology Whole Prostate VL5_UNC    26753400    886    3340  2670   8     3     6.16013
Pathology Stomach Biopsy VL6_UNC     1102248    902     486   756   8     3     4.53285

Note that Bits is the official number of bits used as
stated by the source of the images ... the dynamic
range of the actual image may not use this much.

Also, the images are stored as 8 or 16 bit words (little
endian), eg. a 12 bit pixel actually occupies 16 bits (in
the least significant bits). This is all described in the
DICOM header, but the TIFF header doesn't preserve this
distinction.

All images are single frame. The color image(s) are all
color-by pixel (ie. RGBRGB...), not color-by-plane.

CHANGES.

2004/08/26

- fix truncated reversible JPEG 2000 VL4, VL5, VL6

2004/01/19

- remove images outside JPEG lossy range, and set bit depth and pixel representation
  correctly for those remaining

2003/12/10

- set >8 bit lossy JPEG component precision to exactly 12 bits (not 10 in some cases)
- set image type to derived, add derivation description and code sequence,
  add source image sequence, add lossy compression ratio

2003/12/08

- set >8 bit lossy JPEG transfer syntax to .51 not .50 correctly

2003/12/06

- make fragment items padded to even length if necessary
- fragment more aggressively to better test decoders
- revise file sizes in README

2003/07/10

- initial release.

