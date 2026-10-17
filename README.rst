**Turn a DICOM series into a NumPy volume**

This is a development fork of `dicom-numpy <https://github.com/innolitics/dicom-numpy>`__, an Innolitics Python library for combining image slices into a three-dimensional NumPy array. Upstream's slice-combination routine also returns an affine transform into DICOM patient coordinates, making it useful when image processing needs both voxel values and spatial context.

**Contribution to review:** `PR #40 <https://github.com/innolitics/dicom-numpy/pull/40>`__ proposes streaming zipped DICOM members into the reader instead of first allocating each complete decompressed entry. The pull request contains the specific read-path change and its validation scope.

Read the `official documentation <http://dicom-numpy.readthedocs.io/en/latest/>`__ for installation, supported series geometry, and API usage. The upstream README follows below. Use the `branch comparison <https://github.com/innolitics/dicom-numpy/compare/master...jdotc1:master>`__ to inspect the default branch separately from the proposed contribution.

----

.. image:: https://travis-ci.org/innolitics/dicom-numpy.svg?branch=master
   :target: https://travis-ci.org/innolitics/dicom-numpy

===========
DICOM Numpy
===========

See `Our Documentation <http://dicom-numpy.readthedocs.io/en/latest/>`_.
