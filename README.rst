=======================
Simple Template Toolkit
=======================

Simple templating for all your simple templating projects


Features
--------

The following exported console script is available for use:

- make-substitutions
- insert-lines


Usage
-----

.. code-block:: python

    from simple_template_toolkit import STTManager

    tm = STTManager()

    tm.make_substitutions(
      template_file=template_file,  # the template file containing your placeholder keys (e.g.: $;PARAM1$;)
      outfile=outfile, # the file that should be written out
      lookup=lookup # a dictionary contain placeholders for keys (e.g.: $;PARAM1$;) and corresponding values (e.g.: xyz) replace with
    )
